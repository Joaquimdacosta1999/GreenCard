# 🇿🇦 K53 SA Open Source Learning Hub

An independent, community-driven platform built to make studying for the South African K53 Learner’s Licence accessible, accurate, and completely free. 

---

## 🎯 Our Mission
**The goal of this project is simple:** to create a comprehensive, crowd-sourced study hub where anyone preparing for their learner's licence test can learn, practice, and test their knowledge. Because traffic regulations and test standards can shift, this platform relies on community participation—allowing contributors from all over South Africa to share updates, refine study materials, and help others succeed.

Every single answer provided in this hub must be strictly backed by official documentation from **The National Road Traffic Act (NRTA)** or **The NaTIS Official Portal**, ensuring total accuracy and trust.

Want to help improve this platform or contribute content? Check out our [CONTRIBUTING.md](./CONTRIBUTING.md) guide to get started!

---

## 🚫 1. Solving the Root Cause (Why We Exist)

Most existing K53 apps and websites are built for aggressive ad-monetisation, not for actual learning retention. They suffer from foundational flaws that we actively reject:
*   **No Paywalls, Ever:** Commercial apps bait users into downloading them, only to lock the crucial 68-question mock exam behind a subscription or an upfront        paywall. This hub will remain 100% free forever.
*   **Zero Invasive Ads:** You cannot study effectively when video ads interrupt you every three questions. This platform enforces a clean, distraction-free studying interface.
*   **The Trust Deficit (Fixed by NaTIS):** Other platforms use unverified or outdated question paraphrases. Every single question here is tied to an explicit legal clause or verified portal link.
*   **Rapid Law Updates:** Other platforms use unverified or outdated question paraphrases. Every single question here is tied to an explicit legal clause or verified portal link.
*   Rapid Law Updates:** When traffic laws or speed regulations change in South Africa, commercial software updates take months. Our open-source repository allows changes to happen instantly via community Pull Requests.

---

## 🛠️ 2. Tech Stack & Software Architecture
We keep our architecture incredibly lightweight and modern so anyone with fundamental web development skills can contribute without friction:
*   **Frontend UI:** Vanilla HTML5, modern CSS3 (Flexbox/Grid layout frameworks), and native JavaScript (ES6+).
*   **Database & API Layer:** Strictly file-based using a human-readable `/data/questions.json` model. This removes the need for complex local database management (like SQL/NoSQL engines) to get started.
*   **CI/CD Pipeline:** Automated continuous deployment via **GitHub Pages** or Vercel. Merging code into the `main` branch updates the live application instantly.

---

## 🚀 3. Quick Start (Run the Project Locally)
Want to run the platform locally on your computer? You can get a development server running in under two minutes:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Joaquimdacosta1999/k53-sa-open-source.git
   ```
2. **Navigate into the directory:**
   ```bash
   cd k53-sa-open-source
   ```
3. **Launch the app:**
   Open the `index.html` file directly in any modern web browser, or use the *Live Server* extension inside VS Code.

---

## 📊 4. Strict NaTIS Verification Schema
To enforce absolute accuracy, every practice question stored inside our `/data/questions.json` file must strictly adhere to the following verified structure:

```json
[
  {
    "id": 1,
    "category": "Rules of the Road",
    "question": "What is the general speed limit on an urban public road, unless indicated otherwise by a sign?",
    "options": ["60 km/h", "80 km/h", "120 km/h"],
    "answer": "60 km/h",
    "verification": {
      "source_name": "NaTIS / National Road Traffic Act",
      "reference_section": "Regulation 292 of the NRTA (Act 93 of 1996)",
      "official_url": "https://natis.gov.za",
      "explanation": "According to the National Road Traffic Act and official NaTIS guidelines, the general speed limit in an urban area is 60 km/h."
    }
  }
]
```
---

## 🎯 5. Core Features Roadmap
*   [ ] **The 68-Question Exam Simulator:** A timed testing engine matching the exact question distribution weight used by official traffic departments.
*   [ ] **Section-Specific Quizzes:** Targeted practice tools focused purely on Road Signs, Rules of the Road, or Vehicle Controls.
*   [ ] **NaTIS Verification Badges:** Clickable UI shields below each question displaying its legal source and rationale.
*   [ ] **Local Progress Persistence:** Utilizing browser `localStorage` to save user test history and highlight weak areas securely on their device without requiring accounts.
*   [ ] **Dark Mode Support:** A built-in accessibility theme designed for late-night study sessions.

---

## 👥 6. How to Contribute (Coders & Non-Coders)
We highly value all forms of contribution. You do not need to be an expert software engineer to make an impact:
*   **For Coders:** Pick up tasks labeled `good-first-issue` on our GitHub Issues page. Help optimize quiz logic, polish CSS responsiveness, or refactor state persistence.
*   **For Content Contributors (Non-Coders):** Help us map out and transcribe official questions, find correct high-quality images of traffic signs, or proofread current entries against updated NaTIS regulations.

---

## 📂 7. Project Directory Structure
```text
k53-learn-to-pass/
├── assets/             # Images, SVGs of Road Signs and Vehicle Controls
├── data/               # Human-readable JSON question banks
│   └── questions.json  # NaTIS verified question array
├── pages/              # Learning documentation and overviews
│   ├── test-overview.html
│   ├── vehicle-controls.html
│   └── rules-of-the-road.html
├─ quiz/               # Interactive test components and modules
└── index.html          # Main application landing page
```
---

## 🔒 8. Project Security & Anti-Spam Policy
Because this is an open public repository for educational content, we maintain high quality-control standards:
*   No external third-party tracking cookies or pixel frameworks are permitted in pull requests.
*   All automated script injections or data modifications will be flagged and rejected by code maintainers.
*   Pull requests changing the `questions.json` dataset will only be approved if the changes include a valid, verifiable link to official documentation.

---

## ⚖️ 9. Open Source Licensing
This project is completely open-source and released under the **MIT License**. You are completely free to fork it, modify it, and run it independently without worrying about legal restrictions or commercial pushback.

---

## Table of Contents

* [1. THE LEARNER'S LICENCE TEST OVERVIEWS](./pages/road-signs.html)
    * [OVERVIEW](./pages/road-signs.html#regulatory)
        * [What is a Learner's licence](./pages/road-signs.html#control)
        * [To pass learner's license test you will need to:](./pages/road-signs.html#command)
        * [What are the minimum age requirements for obtaining a learner's licence?](./pages/road-signs.html#prohibition)
        * [What can disqualify me from obtaining a learner's Licence?](./pages/road-signs.html#reservation)
        * [What will I need when I apply?](index.html)
        * [What will the learner's licence authorize me to do?](./index.html)
        * [How long is a learner's license valid for?](index.html)
        * [How will I tested?](./index.html)
        * [What is the pass mark in the official test?](./index.html)
        * [Be sure you understand the test question](./index.html)

* [2. THE CONTROLS OF THE VEHICLE](index.html)
    * [OVERVIEW](./index.html)
        * [Motor vehicle controls](./index.html)
        * [Combining the use of vehicle controls (Automatic vehicles do not have a clutch)](index.html)
        * [All vehicles and motorcycles](./index.html)
        * [Combining use of vehicle controls](./index.html)

* [3. DEFENSIVE DRIVING THE K53 WAY](./index.html)
    * [OVERVIEW](./index.html)
        * [Basic elements of the K53 defensive driving standard](./index.html)
        * [Keep a safe following distance](./index.html)
        * [Use the mirrors correctly](./index.html)
        * [Check in the blind spots](./index.html)
        * [Signal your intention](./index.html)
        * [Use the clutch correctly](./index.html)
        * [Use the steering correctly](./index.html)
        * [Control your speed properly](./index.html)
        * [Use the breakes correctly](./index.html)

* [4. ROAD SIGNS OVERVIEW](./index.html)
    * [OVERVIEW](./index.html)
        * [Purpose](./index.html)
        * [How signs are presented](./index.html)
        * [Sign groupings](index.html)
        * [Temporary signs](./index.html)
        * [Symbols](./index.html)

* [5. REGULATORY SIGNS](./index.html)
    * [OVERVIEW](./index.html)
        * [cotrol signs: to control traffic how](./index.html)
        * [Command signs: to give instructions](./index.html)
        * [Prohibiton signs: to prohibit certain sections to classes of vehicles](./index.html)
        * [Reservation signs: to reserve lanes, roadways (R) or parking areas (P)](./index.html)
        * [Limit prohibition signs: to set specific limits permitted on the road, where exceeding such limit is prohibited](./index.html)
        * [Comprehensive signs: to indicate comprehensive rules](./index.html)
        * [De-restriction signs: to cancel restrictions](./index.html)
        * [Selective restiction regulatory signs: to apply the rules selectively](./index.html)
        * [Traffic signals: to control traffic flow](./index.html)
    * [REGULATORY SIGNS: QUESTIONS AND ANSWERS](./index.html)

* [6. WARNING SIGNS](./index.html)
    * [OVERVIEW](./index.html)
        * [Road situations ahead](./index.html)
        * [Traffic control ahead](./index.html)
        * [Changes in vehicle movement ahead](./index.html)
        * [Road Layout changes ahead](./index.html)
        * [Moving hazards ahead](./index.html)
        * [Hazard marker plates](index.html)
        * [Examples of warning sign combinations](./index.html)
    * [WARNING SIGNS: QUESTIONS AND ANSWERS](./index.html)

* [7. INFORMATION SIGNS](./index.html)
    * [OVERVIEW](./index.html)
        * [Signs](index.html)
    * [INFORMATION SIGNS: Questions and answers](./index.html)

* [8. GUIDANCE SIGNS](index.html)
    * [OVERVIEW](index.html)
        * [GUidance sign colour combinations](./index.html)
        * [Location name symbols](./index.html)
        * [Location name examples](./index.html)
        * [Direction sign symbols](./index.html)
        * [Local direction sign symbols](./index.html)
        * [Tourism sign symbols](./index.html)
        * [Direction sign examples](./index.html)
        * [Diagrammatic signs](./index.html)
    * [GUIDANCE SIGNS: Questions and answers](./index.html)

* [9. ROAD SURFACE MARKINGS](index.html)
    * [OVERVIEW](./index.html)
        * [Regulatory markings](./index.html)
        * [Warming and guidance markings](./index.html)
    * [ROAD SURFACE MARKINGS: Questions and answers](index.html)

* [9. RULES OF THE ROAD](./index.html)
    * [OVERVIEW](./index.html)
        * [General](./index.html)
        * [Maximum speed limits](./index.html)
        * [DIvided roads](./index.html)
        * [Overtaking another vehicle](./index.html)
        * [Overtaking on the left](./index.html)
        * [Passing Oncoming vehicles](./index.html)
        * [Being overtaken](./index.html)
        * [ROad shoulders](#-k53-sa-open-source-learning-hub)
        * [Dedicated public transport lanes](./index.html)
        * [Traffic circles](#)
        * [Crossing or entering a road or traffic lane](#)
        * [Driving signals](#)
        * [Hand signal](#)
        * [Turning at intersections](#)
        * [Parking](#)
        * [Some no-stopping and no-parking distances](#)
        * [Other no-stopping places](#)
        * [Other no-parking place](#)
        * [Stopping on the road](#)
        * [Compulsory stops](#)
        * [Lights](#)
        * [Towing](#)
        * [Not allowed on freeways](#)
        * [Vehicles causing excessive noise](#)
        * [Use of a hooter](#)
        * [Pedestrians' right of way at a pedestrian crossing](#)
        * [Learner drivers on freeways](#)
        * [Being overtaken on a freeway](#)
        * [General duties of drivers and passengers](#)
        * [Racing and sport](#)
        * [Abandoned vehicles](#)
        * [Hindering or obstructing traffic](#)
        * [Pedestrians' legal rights](#)
        * [Damage to public roads](#)
        * [Accidents/collisions](#)
        * [Reckless, negligent, or inconsiderate driving](#)
        * [Tyres](#)
        * [Intoxicating liquor and narcotic drugs](#)
        * [Conveying passengers](#)
        * [Seat belts](#)
        * [Carrying loads on motor vehicles](#)
        * [Animals on public roads](#)
        * [Emergency](#)
        * [Anauthorized use of a vehicles](#)
        * [Additional rules specifically for motorcycles, motor-tricycles and quad-bikes](#)
    * [RULES OF THE ROAD: Questions and answers](#)


## 🏛️ Official Government References
Every topic mapped above complies with South African traffic standards via the NaTIS Official Portal. All study material directly correlates with the National Road Traffic Act (Act 93 of 1996).**[NaTIS Official Portal](https://www.natis.gov.za/)**.