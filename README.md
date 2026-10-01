# Xuber SPOF Training Suite

**Interactive training portal for Xuber Enterprise critical Single Points of Failure (SPOFs)**

🎓 **24 modules across 4 teams** | 📚 **3-level learning paths** | 🚀 **Self-contained, no backend required**

## Visit the Portal

**👉 [Launch Training Portal](https://dwatson34.github.io/spof-training/)**

---

## What's Included

### XE Team — 10 Modules
- **Xuber HTMLUI (3 levels)** — Frontend framework architecture, service patterns, component structure
- **Claim Transactions (3 levels)** — Transaction model, financial framework, layer claims
- **Angular Engineering (4 modules)** — Foundation, Advanced, HTMLUI in Practice, Testing & CI

### XIAP Framework — 3 Modules ⭐ NEW
- **Beginner** — Plugin architecture, lifecycle points, configuration
- **Intermediate** — Plugin interfaces, context access, error handling
- **Expert** — Advanced predicates, decision tables, ObjectFactory services

### Release Management — 7 Modules
- AWS Services | iSeries/DB2 | Azure Pipelines & CI/CD
- SQL & Database Refresh | SOLR & K2 Scheduler
- DR & Certificates | Xuber Patches

### Genius Team — 4 Modules
- Genius Rating | SmartTest Testing
- Bureau Processing | Intercept Messaging

---

## Documentation

All documentation is included in this repository:

1. **[User Guide](XUBER_SPOF_TRAINING_USER_GUIDE.md)** — How to take modules, scoring, learning paths
2. **[Technical Documentation](XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md)** — Architecture, deployment, extending for new teams
3. **[Module Creation Prompt](SPOF_Training_Module_Creation_Prompt.md)** — Template for building new training modules

---

## Key Features

✅ **Interactive Learning**
- 7-8 slides per module with animations
- 10-question quiz per module (70% pass threshold)
- Scenario challenges (Intermediate & Expert levels)
- SVG flow diagrams showing system architecture

✅ **Accessibility**
- Text-to-speech narration for all slides
- Keyboard navigation (arrow keys)
- High-contrast color scheme
- Mobile-responsive design

✅ **No Backend Required**
- Static HTML files only
- Free GitHub Pages hosting
- Progress tracking via browser LocalStorage
- Works offline after initial load

✅ **Easy to Extend**
- Template prompt for new teams
- Proven 3-level structure
- Self-contained HTML modules (no build process)
- Documented code examples from real Xuber codebase

---

## Quick Start

### For Learners
1. Visit [the portal](https://dwatson34.github.io/spof-training/)
2. Select a module that interests you
3. Click through slides (use arrow keys or buttons)
4. Complete the quiz (10 questions, 70% to pass)
5. Progress is saved in your browser

### For Teams Building New Modules
1. Read [XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md](XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md)
2. Use [SPOF_Training_Module_Creation_Prompt.md](SPOF_Training_Module_Creation_Prompt.md)
3. Brief Claude with:
   - Source files (TypeScript, C#, config)
   - Architecture overview
   - API documentation
   - Test fixtures
4. Claude builds 3-level modules in 2-3 hours
5. Deploy to GitHub (automatic GitHub Pages hosting)

---

## By the Numbers

- **24 modules** across 4 teams
- **~1.9 MB** total payload (all modules + portal)
- **7-8 slides** per module
- **10 quiz questions** per module
- **4 scenario challenges** per Intermediate/Expert module
- **~45-75 minutes** per module to complete
- **0 backend services** required
- **0 databases** needed
- **Free hosting** via GitHub Pages

---

## Recommended Learning Paths

### For New XE Developers
1. HTMLUI Beginner → Intermediate → Expert
2. Angular Foundation → Advanced
3. Claim Transactions Beginner → Intermediate

### For Plugin Developers
1. XIAP Beginner → Intermediate → Expert

### For Release Management
1. Infrastructure modules (AWS, iSeries, Azure)
2. Data Management (SQL, SOLR)
3. Operations (DR, Patches)

### For Genius Team
1. Genius Rating
2. SmartTest
3. Bureau Processing
4. Intercept Messaging

---

## Architecture

```
GitHub Pages (Static Hosting)
    ↓
index.html (Portal Dashboard)
    ├─ 24 Module Cards
    ├─ Progress Tracking (LocalStorage)
    └─ Team Filtering
    ↓
Module HTML Files (Self-Contained)
    ├─ Slides (7-8 per module)
    ├─ Quiz (10 questions)
    ├─ Scenarios (Intermediate/Expert)
    └─ Animations (SVG)
```

**Technology Stack:**
- HTML5 + CSS3 + JavaScript (no frameworks)
- SVG animations (inline)
- Web Speech API (TTS narration)
- Browser LocalStorage (progress tracking)

---

## Quality Assurance

All modules include:
- ✅ Real code examples from Xuber codebase
- ✅ Text-to-speech narration for accessibility
- ✅ Interactive animations showing system flow
- ✅ 10-question quiz per module
- ✅ Scenario challenges (Intermediate/Expert)
- ✅ High-contrast color schemes
- ✅ Mobile-responsive design
- ✅ Keyboard navigation support

---

## Deployment

### Initial Setup
```bash
git clone https://github.com/dwatson34/spof-training.git
cd spof-training
```

### Update Modules
```bash
# Copy new/updated HTML files
cp path/to/v2_*.html .
cp path/to/index.html .

# Commit and push (GitHub Pages auto-deploys)
git add .
git commit -m "Update modules"
git push origin main
```

**Note:** GitHub Pages takes 30 seconds to rebuild after push.

### Add a New Module
1. Follow the **Module Creation Prompt**
2. Place HTML file in repository root
3. Update `index.html` with new card + KEYS array
4. Push to GitHub (automatic deployment)

---

## Support & Contribution

### Found a Bug?
- File an issue on GitHub
- Include: module name, browser, exact steps to reproduce

### Want to Add a Module?
- Use the **Module Creation Prompt** to build it
- Submit a pull request with:
  - New module HTML file
  - Updated index.html
  - Documentation (in comments)

### Have Feedback?
- Check the **User Guide** for common questions
- Read **Technical Docs** for architecture details
- Pull requests welcome!

---

## Version History

**v1.0 (Released October 2026)**
- 24 modules across 4 teams
- Complete XIAP Framework training (new)
- All modules reorganized with subsections
- Text-to-speech for all modules
- Interactive scenario challenges (Intermediate & Expert)
- Comprehensive documentation

---

## License & Attribution

Built with real Xuber Enterprise source code and official technical documentation (Release 26.3).

Training materials synthesize complex systems into interactive, digestible learning modules.

---

## Next Steps

1. **Take a module** → Visit [the portal](https://dwatson34.github.io/spof-training/)
2. **Build for your team** → Read [Technical Docs](XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md)
3. **Share feedback** → File a GitHub issue or pull request
4. **Spread the word** → Share the portal link with your team

---

**Questions?** Check the [User Guide](XUBER_SPOF_TRAINING_USER_GUIDE.md) or [Technical Docs](XUBER_SPOF_TRAINING_TECHNICAL_DOCS.md).

**Ready to learn?** 👉 [Launch Training Portal](https://dwatson34.github.io/spof-training/)
