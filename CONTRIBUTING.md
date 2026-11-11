# Contributing to GreenCard 🇿🇦

First off, thank you for taking the time to contribute!  

**GreenCard** is a free, community-driven open-source platform that helps South Africans prepare for the K53 Learner’s Licence test. Every contribution — whether it’s a single question, a road sign explanation, a bug fix, or a new feature — helps someone pass their test without paying for expensive apps.

We welcome contributions from everyone: learners, driving instructors, developers, designers, and people who simply care about road safety.

---

## Table of Contents

- [Ways You Can Contribute](#ways-you-can-contribute)
- [Label Meanings](#label-meanings)
  - [Type Labels](#type-labels)
  - [Status Labels](#status-labels)
  - [Priority Labels](#priority-labels)
  - [Special Labels](#special-labels)
- [How to Contribute (Step-by-Step)](#how-to-contribute-step-by-step)
- [Content Contribution Guidelines](#content-contribution-guidelines)
- [Code Contribution Guidelines](#code-contribution-guidelines)
- [Pull Request Process](#pull-request-process)
- [Code of Conduct](#code-of-conduct)

---

## Ways You Can Contribute

You do **not** need to be a developer to contribute.

### 1. Content & Knowledge
- Transcribe and structure content from the official K53 manual
- Write clear explanations for road signs (Regulatory, Warning, Guidance, Information)
- Break down Rules of the Road, Vehicle Controls, and Defensive Driving (K53 method)
- Add new practice questions with correct answers and official references
- Update content when NaTIS / Department of Transport regulations change

### 2. Code & Features
- Improve the quiz engine (timed tests, section quizzes, progress tracking)
- Fix bugs or improve mobile responsiveness
- Add Dark Mode, better accessibility, or performance improvements
- Help with GitHub Pages deployment or project structure

### 3. Design & Assets
- Create or improve SVG/PNG road sign images
- Improve the visual design and user experience
- Make the site more accessible (colour contrast, screen readers, etc.)

### 4. Community & Documentation
- Improve this CONTRIBUTING.md or the README
- Report outdated or incorrect information
- Help triage issues and welcome new contributors

---

## Label Meanings

We use labels to organise issues and pull requests. This makes it easy for everyone to find work that matches their skills and interest.

### Type Labels

| Label | Meaning |
|-------|---------|
| `type: content` | Adding or improving study material, questions, explanations, or road signs |
| `type: bug` | Something is broken or incorrect |
| `type: enhancement` | New feature or improvement to existing functionality |
| `type: documentation` | Improving README, CONTRIBUTING, or other docs |
| `type: design` | Visual design, UI/UX, or asset improvements |
| `type: question` | General questions about the project or K53 content |

### Status Labels

| Label | Meaning |
|-------|---------|
| `status: needs-triage` | New issue that has not been reviewed yet |
| `status: ready` | Confirmed and ready for someone to work on |
| `status: in-progress` | Someone is currently working on it |
| `status: blocked` | Cannot proceed until something else is resolved |
| `status: needs-review` | Waiting for feedback or approval |
| `status: needs-verification` | Content that needs official NaTIS / NRTA confirmation |

### Priority Labels

| Label | Meaning |
|-------|---------|
| `priority: critical` | Blocks learning or contains incorrect official information |
| `priority: high` | Important improvement or widespread issue |
| `priority: medium` | Nice to have, should be done soon |
| `priority: low` | Minor improvement or polish |

### Special Labels

| Label | Meaning |
|-------|---------|
| `good first issue` | Perfect for new contributors |
| `help wanted` | Extra attention needed — community help appreciated |
| `verified` | Content has been checked against official NaTIS / NRTA sources |
| `needs images` | Requires road sign or vehicle control images |
| `duplicate` | Already covered by another issue |

---

## How to Contribute (Step-by-Step)

### For First-Time Contributors

1. **Fork** the repository  
   Click the **Fork** button at the top right of the [GreenCard repository](https://github.com/Joaquimdacosta1999/GreenCard).

2. **Clone your fork**
   ```bash
   git clone https://github.com/YOUR-USERNAME/GreenCard.git
   cd GreenCard
   ```

3. **Create a new branch**
   ```bash
   git checkout -b type/short-description
   # Examples:
   # git checkout -b content/add-regulatory-signs
   # git checkout -b fix/quiz-timer-bug
   # git checkout -b docs/update-contributing
   ```

4. **Make your changes**

5. **Commit your changes**
   ```bash
   git add .
   git commit -m "type: short clear description of what you did"
   ```

6. **Push to your fork**
   ```bash
   git push origin your-branch-name
   ```

7. **Open a Pull Request**
   Go to the original GreenCard repository and click **Compare & pull request**.

---

## Content Contribution Guidelines

This is the most important section for accuracy.

### Rules for all content

- Every answer and explanation **must** be backed by official sources:
  - National Road Traffic Act (Act 93 of 1996)
  - National Road Traffic Regulations
  - Official NaTIS portal (https://www.natis.gov.za)
- Always include a verification block when adding or changing questions.
- Prefer clear, simple language that a first-time learner can understand.
- Do not copy copyrighted material word-for-word from commercial K53 books.

### Recommended structure for practice questions

```json
{
  "id": 42,
  "category": "Rules of the Road",
  "question": "What is the general speed limit on an urban public road unless otherwise indicated?",
  "options": ["60 km/h", "80 km/h", "100 km/h", "120 km/h"],
  "answer": "60 km/h",
  "verification": {
    "source_name": "National Road Traffic Act",
    "reference_section": "Regulation 292",
    "official_url": "https://www.natis.gov.za",
    "explanation": "According to Regulation 292 of the NRTA, the general speed limit in an urban area is 60 km/h unless a different limit is indicated by a road sign."
  }
}
```

### When adding road sign content

- Include the official name of the sign
- Explain what the driver must do
- Note any exceptions
- Ideally include a clear image or SVG of the sign

---

## Code Contribution Guidelines

- Keep the tech stack simple: **Vanilla HTML, CSS, and JavaScript** (no heavy frameworks unless discussed first)
- Prefer readable code over clever code
- Make sure the site works well on mobile phones
- Test your changes locally by opening `index.html` in a browser
- Avoid adding external tracking scripts or unnecessary dependencies

---

## Pull Request Process

1. Link your PR to an existing issue if one exists (`Closes #123`)
2. Give your PR a clear title (e.g. `content: add 15 new Rules of the Road questions`)
3. Describe what you changed and why
4. For content changes, mention the official source you used
5. A maintainer will review your PR. We may ask for small changes — this is normal and helps keep quality high.

---

## Code of Conduct

- Be respectful and patient — many contributors are beginners
- Focus on the content and the goal of helping learners
- No spam, self-promotion, or off-topic discussions
- Incorrect information that could mislead learners will be corrected or rejected

---

Thank you for helping make free, high-quality K53 study material available to every South African.  

Every contribution counts.  
Let’s help more people get their Green Card the right way. 🚗🇿🇦