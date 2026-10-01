# Xuber SPOF Training Suite — User Guide

## Overview

The **Xuber SPOF Training Suite** is an interactive, web-based training platform designed to help developers, architects, and technical staff understand and master the critical Single Points of Failure (SPOFs) in the Xuber Enterprise system.

**Current Version:** 1.0  
**Total Modules:** 24  
**Teams Covered:** XE (10 modules), XIAP (3 modules), RM (7 modules), Genius (4 modules)  
**Knowledge Cutoff:** Based on Xuber Enterprise Release 26.3

---

## What's Included

### XE Team Modules (10)
**Xuber HTMLUI (3 levels)**
- Beginner: HTMLUI basics, folder structure, request flow
- Intermediate: XuWebApiManager internals, service patterns, complete endpoint references
- Expert: Adding service methods, feature module structure, advanced debugging

**Claim Transactions (3 levels)**
- Beginner: Transaction concepts, 8 modes, startup sequence, shared templates
- Intermediate: Base class patterns, XuDeferred, 16 injected services, transitions
- Expert: R&P financial framework, layer claims, new transaction types

**Angular Engineering (4 modules)**
- Angular Foundation: Architecture, components, DI, services, routing
- Angular Advanced: Change detection, lifecycle hooks, reactive forms, optimization
- HTMLUI in Practice: Codebase tour, local setup, debugging, git workflows
- Angular Testing & CI: Jasmine, TestBed, code coverage, Azure Pipelines

### XIAP Framework Modules (3)
**New!** Complete plugin development training

- Beginner: What XIAP is, plugin architecture, lifecycle points, configuration
- Intermediate: Plugin interfaces, context access, error handling, Process Handlers
- Expert: Advanced predicates, decision tables, ObjectFactory services, performance

### Release Management Modules (7)
**Infrastructure:** AWS, iSeries/DB2, Azure Pipelines & CI/CD  
**Data Management:** SQL & Database Refresh, SOLR & K2 Scheduler  
**Operations:** DR & Certificates, Xuber Patches

### Genius Team Modules (4)
**Core Systems:** Genius Rating, Genius Bureau Processing  
**Testing & Messaging:** Testing Genius using SmartTest, Genius Intercept Messaging

---

## How to Use

### Accessing the Portal

1. **Navigate to the portal:** `https://dwatson34.github.io/spof-training/`
2. **View the dashboard** showing overall progress (0 of 24 modules passed)
3. **Click on any module card** to enter the training

### Taking a Module

Each module consists of:

- **Slides (7-8 per module)** — Core learning material with text and diagrams
- **Animations** — Interactive flow diagrams showing system architecture and processes
- **Quiz (10 questions per module)** — Multiple choice to test understanding
- **Scenario Challenges** — Real-world problems to solve (Intermediate and Expert levels)

### Navigation

- **Next/Previous buttons** or **arrow keys** to move between slides
- **Progress bar** shows your position in the module
- **Quiz section** on the right sidebar — complete as you read
- **Slide counter** (e.g., "1 / 8") shows current position

### Scoring

- Complete a module by reading all slides and answering the quiz
- **Quiz passes at 70%** (7 out of 10 questions correct)
- Progress is tracked in the portal dashboard
- **Overall progress** shows how many modules you've passed

---

## Module Structure

### Level 1 — Beginner
**Duration:** ~45 minutes per module  
**Target Audience:** New developers, technical leads, anyone needing foundational knowledge

Covers:
- Core concepts and terminology
- Architecture and integration patterns
- Basic configuration and setup
- How to get started

**Example:** HTMLUI Beginner explains what HTMLUI is, the folder structure, how a request flows, and how to read a service file.

### Level 2 — Intermediate
**Duration:** ~60 minutes per module  
**Target Audience:** Developers building features, architects designing components

Covers:
- Detailed code patterns and implementations
- Real code examples from production Xuber codebase
- Complete API references and service tables
- Common patterns and best practices
- 4 scenario challenges to test understanding

**Example:** HTMLUI Intermediate dives into XuWebApiManager internals, shows all 6 service patterns, includes a complete table of XuClaimsService endpoints, and presents real source code examples.

### Level 3 — Expert
**Duration:** ~75 minutes per module  
**Target Audience:** Senior developers, architects, SPOF owners

Covers:
- Advanced patterns and edge cases
- Performance optimization
- Production complexity and real-world scenarios
- 4 expert scenario challenges with complex requirements

**Example:** XIAP Expert covers advanced plugin predicates, decision table logic, ObjectFactory service resolution, and real-world performance considerations.

---

## Key Features

### Interactive Learning
- **Animated flows** showing system execution paths
- **Code blocks** with real examples from Xuber codebase
- **Reference tables** for quick lookup during development
- **Scenario challenges** with answer explanations

### Accessibility
- **Text-to-speech narration** for each slide
- **High-contrast colors** for readability
- **Keyboard navigation** (arrow keys work)
- **Mobile-responsive** design

### Tracking & Progress
- **Module completion** tracked automatically
- **Quiz scores** recorded (70% pass threshold)
- **Overall progress dashboard** shows training completion
- **Filterable by team** (XE, XIAP, RM, Genius)

---

## Prerequisites

### Before Starting
- Working knowledge of the relevant technology stack
  - **XE modules:** C#, .NET, TypeScript/Angular, XML configuration
  - **XIAP modules:** C#, .NET 4.0, OOP principles
  - **RM modules:** DevOps concepts, database management, cloud infrastructure
  - **Genius modules:** Business processes, underwriting/claims concepts

- Familiarity with Xuber business domain (transactions, components, products)

---

## Recommended Learning Path

### For New XE Developers
1. **HTMLUI Beginner** (foundation)
2. **HTMLUI Intermediate** (deepen knowledge)
3. **HTMLUI Expert** (master patterns)
4. **Angular Foundation** (learn Angular basics)
5. **Claim Transactions Beginner** (understand transaction model)
6. **Claim Transactions Intermediate** (implement features)

### For Plugin Developers
1. **XIAP Beginner** (understand framework)
2. **XIAP Intermediate** (learn plugin interfaces)
3. **XIAP Expert** (master advanced patterns)

### For Release Management
1. **Infrastructure modules** (AWS, iSeries, Azure)
2. **Data Management modules** (SQL, SOLR)
3. **Operations modules** (DR, Patches)

### For Genius Team
1. **Genius Rating** (rating engine)
2. **SmartTest** (testing framework)
3. **Bureau Processing** (intercept system)
4. **Intercept Messaging** (messaging patterns)

---

## Common Questions

### Q: Can I retake a module?
**A:** Yes. Your progress is based on the latest quiz attempt. Retake any module to improve your score.

### Q: What if I don't pass the quiz?
**A:** Review the slides and scenario challenges, then retake. The material is cumulative — understanding Beginner is essential for Intermediate.

### Q: Are the scenarios graded?
**A:** No. Scenarios are for learning. Read the answer explanations to understand production patterns.

### Q: Can I download modules?
**A:** Each module is a standalone HTML file. You can save it locally or access via the GitHub Pages portal.

### Q: Is there a certificate?
**A:** Currently no formal certificate, but you can track completion in the portal dashboard.

### Q: How often are modules updated?
**A:** Modules are version-controlled on GitHub. Check for updates when new Xuber releases come out.

---

## Support & Feedback

### Reporting Issues
- Found a mistake? File an issue on GitHub
- Have a question? Check the module slides first
- Want a new module? Request it on the project GitHub

### Suggesting Improvements
- Module too long/short?
- Quiz too easy/hard?
- Missing key concepts?
- Pull requests welcome on GitHub

---

## Technical Details

### Technology Stack
- **Frontend:** Pure HTML5, CSS3, JavaScript (no frameworks)
- **Interactive Elements:** SVG animations, interactive flows
- **Audio:** Text-to-speech narration (browser native)
- **Hosting:** GitHub Pages (static site)
- **Storage:** Browser local storage (progress tracking)

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### File Sizes
- **Beginner modules:** ~25KB each
- **Intermediate modules:** ~26KB each
- **Expert modules:** ~24KB each
- **Index:** ~50KB

---

## Version History

**v1.0 (Released October 2026)**
- 24 modules across 4 teams
- Complete XIAP Framework training (new)
- All XE, RM, Genius modules updated with subsection organization
- Text-to-speech for all modules
- Interactive scenario challenges (Intermediate & Expert)

---

## Next Steps

1. **Start with Beginner modules** for your team
2. **Complete quiz** at end of each module
3. **Review scenario challenges** before moving to Intermediate
4. **Progress to higher levels** as your understanding deepens
5. **Check back regularly** for new modules and updates

---

**For more information, visit:** https://github.com/dwatson34/spof-training

**Questions?** Check the module slides first — most answers are there.

---

*This training suite was built using real Xuber Enterprise source code and official technical documentation. All code examples are from production systems.*
