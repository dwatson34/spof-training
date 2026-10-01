# SPOF Training Module Creation Prompt

Use this prompt when requesting Claude to build interactive SPOF training modules similar to the Xuber SPOF Training Suite.

---

## Your Brief to Claude

**Project:** Build a 3-level SPOF training programme (Beginner → Intermediate → Expert)

**Team/SPOF Details:**
- Team name: [e.g., "Release Management"]
- SPOF classification: [Critical SPOF / High SPOF]
- Module topic: [e.g., "AWS Services", "Database Refresh", "SmartTest"]
- Integration points: [Brief description of how this SPOF integrates with the main system]

**Content Requirements:**
Include all of the following across the 3 levels:
- Architecture and how the system integrates with [parent system]
- Building/configuring components
- API endpoints and payloads (if applicable)
- Configuration samples and best practices
- Testing interactions and validation approaches
- Real-world scenarios and troubleshooting

**Level Progression:**
- **Beginner (Level 1):** Concepts, terminology, what the system is, basic setup, 7 slides, 10-question quiz
- **Intermediate (Level 2):** How it works internally, real code/config examples, patterns, 8 slides, 10-question quiz, 4 scenario challenges
- **Expert (Level 3):** Advanced patterns, edge cases, integration complexity, performance, 8 slides, 10-question quiz, 4 expert scenarios

**Source Materials to Upload:**
Provide ALL of the following:
1. **TypeScript/Code source files** — core services, components, interfaces, types
2. **Configuration files** — JSON/YAML schemas, environment configs, integration setup
3. **API documentation** — endpoint specs, request/response DTOs, example payloads
4. **Real component examples** — actual code from production components
5. **Test fixtures/mocks** — sample data, test scenarios
6. **Architecture diagrams or README** — integration overview, data flow
7. **Any documentation** — design decisions, known issues, troubleshooting guides

**Delivery Format:**
- Three self-contained HTML files (one per level)
- Bureau-style interactive format with:
  - Slides with clear learning progression
  - Code/config blocks extracted from real source
  - Animated flow diagrams showing system interactions
  - Multiple-choice quiz questions (10 per level)
  - Scenario challenges (4 per Intermediate & Expert levels)
  - Text-to-speech narration for accessibility

**Reference Implementation:**
See the completed XE modules in the Xuber SPOF Training Suite:
- HTMLUI (3 levels) — built from real TypeScript source files
- Claim Transactions (3 levels) — built from real component source
- Each uses the same Bureau CSS/JS framework and interactive patterns

---

## How to Request This

When you have your source materials ready, provide Claude with:

1. This prompt (to set expectations)
2. Your team/SPOF details (name, classification, integration points)
3. All source files listed above (upload as files)
4. Any specific learning objectives or pain points to address
5. Reference to the Xuber SPOF Training Suite for style/format examples

Claude will then build your 3-level programme using the same proven methodology.

---

## Key Success Factors

✓ **Real source code** — The best modules are built from actual codebase examples  
✓ **Complete materials** — Having all documentation and config files upfront prevents gaps  
✓ **Clear integration story** — Explain how this SPOF connects to the broader system  
✓ **Scenario design** — Include real failure cases and edge cases from your domain  

Without source materials, modules will be generic and lack the depth that makes training valuable.
