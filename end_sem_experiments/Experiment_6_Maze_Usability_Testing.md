# Experiment 6: Unmoderated Usability Testing with Maze

- **Student Name:** Nisarg Malhotra
- **Roll Number:** 29
- **PRN:** 1262243207
- **Class / Batch:** TY AI_DS Panel-F, Batch-F2
- **Project Tested:** MalhotraUPI — UPI Payment App Prototype
- **Date of Submission:** 02 November 2026

---

## 1. Aim
To study how an unmoderated remote usability testing tool such as Maze can be used to evaluate a clickable Figma prototype, identify usability problems, and collect task-based feedback for MalhotraUPI.

---

## 2. Problem Statement
Study the use of Maze for testing a UPI payment application prototype created in Figma. Evaluate whether users can discover important features, complete common payment-related tasks, and understand transaction information without assistance.

---

## 3. References
- [Maze Official Platform](https://maze.co/)
- [Maze Documentation & Guides](https://help.maze.co/)

---

## 4. Theory & Key Testing Terminology
Maze is a remote usability testing platform that allows designers to test clickable prototypes with participants without building a working application. A Figma prototype can be imported into Maze using its share link. The designer creates missions, defines the expected path and end screen, shares a test link, and reviews the quantitative and qualitative results collected from participants.

| Term | Meaning |
| :--- | :--- |
| **Mission** | A task given to a participant, with a defined starting screen and completion point. |
| **Expected Path** | The sequence of prototype screens intended to complete a mission. |
| **Direct Success** | The participant reaches the defined end screen through the expected path. |
| **Indirect Success** | The participant reaches the end screen using a different route. |
| **Give-up / Bounce** | The participant leaves a mission without reaching its end screen. |
| **Misclick** | A click on a screen area that is not linked to the intended interaction. |
| **Heatmap** | A visual overlay showing where participants clicked on a screen. |
| **Time on Task** | The time taken by a participant to complete a mission. |

---

## 5. Test Plan & Missions

| ID | Mission Shown to Participant | Expected Path (Figma Frame Names) | Design Aspect Tested | Success Reaches |
| :---: | :--- | :--- | :--- | :--- |
| **M1** | You need to pay a shopkeeper. Find the QR scanner and reach the scan screen. | `01 Home` $\rightarrow$ `02 Scan & Pay` $\rightarrow$ `03 QR Scanner` | Discoverability of primary QR payment action | `03 QR Scanner` |
| **M2** | Send ₹250 to a saved contact. Review the details before confirming the demo payment. | `01 Home` $\rightarrow$ `04 Send Money` $\rightarrow$ `05 Select Contact` $\rightarrow$ `06 Enter Amount` $\rightarrow$ `07 Payment Review` | Clarity of send-money flow and payment review | `07 Payment Review` |
| **M3** | You want to check whether your previous payment was successful. Find the transaction history and open a transaction. | `01 Home` $\rightarrow$ `08 History` $\rightarrow$ `09 Select Transaction` $\rightarrow$ `10 Transaction Details` | Discoverability and readability of transaction records | `10 Transaction Details` |
| **M4** | You want to check which bank account is linked to MalhotraUPI. Find the bank-account section. | `01 Home` $\rightarrow$ `11 Profile` $\rightarrow$ `12 Bank Accounts` $\rightarrow$ `13 Account Details` | Navigation and account settings discoverability | `13 Account Details` |
| **M5** | You want to see your personal details and app settings. Open the relevant section. | `01 Home` $\rightarrow$ `11 Profile` $\rightarrow$ `14 Settings` | Clarity of profile navigation and labels | `14 Settings` |

---

## 6. Test Results & Metrics

### A. Participant Summary
- **Participants Started:** 6 (All reached landing frame)
- **Participants Completed:** 5 (1 dropped off at M4)
- **UPI Experience:** 83.3% Regular Users (4 Daily, 1 Several times a week, 1 Occasionally)
- **Report Export Date:** 02 November 2026

### B. Mission Performance Breakdown

| Mission | Responses | Success % | Drop-off % | Misclick % | Avg. Time (s) | Ease Avg. (1–5) |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **M1: Scan QR** | 6 | 100% | 0% | 8.3% | 14.2s | **4.8 / 5** |
| **M2: Send ₹250** | 6 | 100% | 0% | 14.5% | 38.6s | **4.4 / 5** |
| **M3: Transaction History** | 6 | 83.3% | 16.7% | 22.1% | 29.4s | **3.8 / 5** |
| **M4: Check Bank Account** | 5 | 80.0% | 20.0% | 35.0% | 45.1s | **3.2 / 5** |
| **M5: Profile & Settings** | 5 | 100% | 0% | 11.2% | 18.0s | **4.6 / 5** |

---

## 7. Heatmap Findings & Usability Bugs

### Screen with Most Misclicks: `01 Home` & `11 Profile`
- **Heatmap Analysis:** During Mission 4, 35% of clicks landed on the non-interactive promotional banner on `01 Home` and the main profile balance card rather than navigating to `12 Bank Accounts`. Participants expected bank account details to be accessible directly from the primary Home dashboard header.
- **Design Remedy:** Added a quick-access "Linked Bank Accounts" pill directly beneath the total balance card on `01 Home`.

### Prioritized Usability Issues
1. **Bank Account Location Nested Too Deep (Severity: Medium):** High misclicks (35.0%) and lowest ease (3.2/5). *Fix:* Expose linked bank account shortcut on main dashboard sub-header.
2. **Filter Tabs in History Confused Users (Severity: Low):** 22.1% misclicks on non-clickable status badges. *Fix:* Make transaction status badges visually distinct from filter pills.
3. **Static Input Delay in Demo (Severity: Medium):** Avg. time on M2 reached 38.6s due to clicking static amount box. *Fix:* Add prompt indicating clicking "Continue" populates pre-filled values.

---

## 8. Qualitative Participant Feedback
> *"The scan and pay button is extremely prominent and easy to reach with one hand. Much cleaner than Paytm."*  
> — **Participant 102948**

> *"It feels light and fast, but I expected my linked bank account to be right next to my balance."*  
> — **Participant 102951**

> *"Overall design is crisp. Simple blue tone makes it feel trustworthy like GPay."*  
> — **Participant 102955**

---

## 9. Conclusion
This study demonstrates how Maze can be used to conduct unmoderated remote usability testing of a Figma prototype for MalhotraUPI. The empirical metrics validate that core everyday payment tasks (Scan & Pay: 100% success, 4.8 ease rating; Send Money: 100% success, 4.4 ease rating) perform exceptionally well, while secondary administrative flows like account linking require shallower navigation hierarchy.

---

## 10. Frequently Asked Questions (FAQs)

### 1. Define the objective of user testing.
The objective of user testing is to evaluate whether people from the target audience can use a product to complete their goals effectively, efficiently, and with reasonable satisfaction. It uncovers confusing layouts, unclear labels, navigation problems, and errors before production release.

### 2. Discuss different methods of user testing.
- **Moderated Testing:** A facilitator observes participants in real-time, asking probing questions.
- **Unmoderated Testing:** Participants complete automated tasks independently (e.g., using Maze).
- **Remote vs. In-Person:** Remote tests on user devices across locations; in-person observes body language in a lab.
- **Think-Aloud Testing:** Participants vocalize their internal thoughts while completing tasks.
- **A/B Testing:** Quantitative comparison between two design variations.

### 3. Explain the features and benefits of Maze.
- **Features:** Direct Figma prototype URL import, automated task mission paths, quantitative tracking (success, bounce, misclicks, time-on-task), click heatmaps, and in-mission opinion surveys.
- **Benefits:** Early validation before development, high scalability with asynchronous testing, and actionable data-driven insights.
