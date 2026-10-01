# Technical Documentation

This guide covers the technical architecture, technology stack, and how to extend the training platform.

---

## System Architecture

The SPOF Training Suite is a self-contained, web-based platform built with vanilla HTML, CSS, and JavaScript. No backend server or database is required.

### How It Works

1. **Landing Page** (`index.html`) — The main entry point with 4 tabs (Jump In, What You'll Get, Teams, Documentation)
2. **Training Modules** (individual HTML files) — Each module is standalone and contains slides, quizzes, and scoring
3. **Module Portal** (`portal.html`) — Optional dashboard showing all 24 modules organized by team
4. **Static Hosting** — Everything runs on GitHub Pages with zero server cost

### Technology Stack

- **Frontend:** HTML5, CSS3, Vanilla JavaScript (no frameworks)
- **Storage:** Browser's local storage for quiz scores
- **Hosting:** GitHub Pages (free, automatic deployment)
- **Version Control:** Git

---

## File Structure

```
spof-training/
├── index.html                              (Landing page with tabs)
├── portal.html                             (Module dashboard)
├── v2_XE_HTMLUI_Beginner_Training.html     (Module)
├── v2_XE_HTMLUI_Intermediate_Training.html (Module)
├── v2_XE_HTMLUI_Expert_Training.html       (Module)
├── ... (21 more modules)
├── README.md                               (Quick start)
├── XUBER_SPOF_TRAINING_USER_GUIDE.md       (User guide)
├── XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md   (This file)
├── DEPLOYMENT_RELEASE_NOTES.md             (Deployment guide)
└── ... (other documentation)
```

---

## Module HTML Structure

Each training module follows this standard structure:

### Head Section
- Meta tags for viewport and charset
- Inline CSS styling (no external stylesheets)
- Title and favicon

### Body Section
- **Header** — Module title and team branding
- **Content Area** — Slides displayed one at a time
- **Navigation** — Previous/Next buttons
- **Quiz Section** — 10 questions with radio buttons
- **Results Section** — Pass/fail message with score

### JavaScript Functions
- `flowStep(slideId, button)` — Navigate to next slide
- `flowReset(slideId)` — Reset to first slide
- `submitQuiz()` — Score the quiz
- `saveScore()` — Store score in localStorage

---

## Key Features

### Interactive Slides
- Each module has 7-8 slides
- Slides contain text, code examples, and learning objectives
- Smooth navigation with Previous/Next buttons
- Progress indicator showing current slide

### Quiz System
- 10 multiple-choice questions per module
- Each question has 4 options
- 70% threshold to pass (7 out of 10 correct)
- Instant feedback on each answer
- Score saved to browser's localStorage

### Text-to-Speech
- Each module has a SLIDE_TTS array with narration text
- Uses browser's built-in Web Speech API
- Optional — users can toggle on/off
- Useful for accessibility and auditory learning

### Progress Tracking
- Quiz scores stored in browser's localStorage
- Scores persist across sessions (unless browser data is cleared)
- Portal dashboard shows completion status
- Module cards show "Completed" or "In Progress" badges

---

## Extending for New Teams

### Step 1: Create a New Module

1. Copy an existing module HTML file
2. Update the module ID, title, and description
3. Replace the slides with your content
4. Write 10 quiz questions
5. Add text-to-speech narration (optional)

### Step 2: Add to Portal

1. Edit `portal.html`
2. Find the modules object in JavaScript
3. Add your new team section or add modules to an existing team
4. Update the module count in the header

### Step 3: Test Locally

1. Open the HTML file in a browser
2. Test all slides, navigation, and quiz
3. Verify scores are saved
4. Check mobile responsiveness

### Step 4: Deploy to GitHub

1. Add files to your Git repository
2. Commit with a descriptive message
3. Push to the main branch
4. GitHub Pages automatically deploys

---

## Customization Guide

### Changing Colors

The suite uses a purple gradient theme. To change:

1. Edit the `<style>` section in `index.html`
2. Look for `--primary-purple: #667eea` and `--secondary-purple: #764ba2`
3. Replace with your brand colors
4. Test in both light and dark modes

### Changing Text

All text (headers, buttons, labels) is directly in the HTML. To customize:

1. Edit the text inside `<h1>`, `<p>`, `<button>` tags
2. No configuration file needed
3. Changes take effect immediately

### Adding New Teams

1. Add a new section in the modules object
2. Define team name, icon, and description
3. Add modules array with your content
4. Update the header to show new team count

---

## Browser Compatibility

The platform works on all modern browsers:

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile Safari (iOS 12+)
- Chrome Mobile (Android 80+)

### Notes
- Older browsers may not support some CSS features
- localStorage is required for score saving
- Web Speech API (for TTS) may not be available in all browsers

---

## Performance Optimization

### Current Optimizations
- Inline CSS and JavaScript (no external requests)
- Minimal DOM manipulation
- No heavy libraries (vanilla JavaScript)
- ~25-200KB per module (easily loaded)

### Tips for Large Deployments
- Host on GitHub Pages (no bandwidth charges)
- Use CDN for assets if adding images
- Compress images to <100KB per module
- Test on slow connections (throttle to 3G in DevTools)

---

## Troubleshooting

### Quiz Scores Not Saving
- Check if localStorage is enabled in browser
- Check browser console for errors (F12)
- Try incognito/private mode

### Slides Not Displaying
- Ensure browser JavaScript is enabled
- Check that HTML file is complete and valid
- Try opening in a different browser

### Text-to-Speech Not Working
- Check if browser supports Web Speech API
- Verify SLIDE_TTS array is defined in HTML
- Check volume settings (system and browser)

---

## Version History

**v1.0** (October 2026)
- Initial release with 24 modules
- 4 teams: XE, XIAP, Release Management, Genius
- Quiz system with localStorage
- Tab-based landing page
- Mobile responsive design

---

## Support

- **GitHub Issues:** https://github.com/dwatson34/spof-training/issues
- **Documentation:** See the links in the Documentation tab
- **Feedback:** Open an issue on GitHub

---

**Last Updated:** October 2026
