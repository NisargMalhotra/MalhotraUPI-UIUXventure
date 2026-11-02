# Experiment 5: Heuristic Evaluation of MalhotraUPI

- **Student Name:** Nisarg Malhotra
- **Roll Number:** 29
- **PRN:** 1262243207
- **Class / Batch:** TY AI_DS Panel-F, Batch-F2
- **System Evaluated:** MalhotraUPI — UPI Payment App Prototype
- **Evaluation Basis:** Prototype Design Review

---

## Part I: Heuristic Evaluation Based on General Interaction Design Principles

**Severity Scale:**  
`0` = No issue | `1` = Cosmetic | `2` = Minor | `3` = Moderate | `4` = Major | `5` = Critical  
*(Lower total severity indicates fewer identified usability issues)*

| S.No. | Heuristic Parameter | Observation / Possible Violation | Severity (0–5) | Ways to Improve |
| :---: | :--- | :--- | :---: | :--- |
| **1** | **Visibility of system status** | The prototype should clearly show whether a payment is being processed, completed, pending or failed. If the design only shows a final success state, users may be unsure what is happening while they wait. | 2 | Add clear loading/progress feedback and distinct Success, Pending and Failed states. Show the latest transaction status and timestamp. |
| **2** | **Match between system and real world** | Labels such as Scan & Pay, Send Money, Bank Account and Transaction History use familiar UPI language. Any technical terms or unclear abbreviations could still confuse first-time users. | 1 | Keep labels familiar and action-oriented. Use plain-language explanations for unfamiliar terms and show currency amounts in a consistent format. |
| **3** | **User control and freedom** | A user may need to go back and correct the recipient or amount before confirming a payment. If the flow does not provide a clear back or edit action, users can feel trapped in the process. | 2 | Provide visible Back and Edit actions before final confirmation. Allow users to cancel a draft payment without losing entered information. |
| **4** | **Consistency and standards** | The blue-and-white visual style and repeated cards support consistency. However, buttons, icons, labels and navigation should behave the same way on every screen. | 1 | Reuse the same button styles, icon meanings, spacing and wording across Home, Payments, History and Profile. Follow familiar UPI interaction patterns. |
| **5** | **Error prevention** | Sending money is a sensitive action. A user could select the wrong contact or enter an incorrect amount if recipient and payment details are not reviewed carefully. | 3 | Show recipient name, UPI ID and amount together on a confirmation screen. Clearly distinguish the primary Pay action from secondary actions. |
| **6** | **Recognition rather than recall** | Prominent shortcuts for Scan & Pay and Send Money reduce the need to remember where common features are located. Recent recipients and recent transactions can further reduce memory effort. | 1 | Keep frequently used actions visible on Home. Use recognisable icons with text labels and show recent recipients or transactions where appropriate. |
| **7** | **Flexibility and efficiency of use** | The focused dashboard is intended to make common actions quick. Frequent users may still benefit from shortcuts, favourite contacts or a quick repeat-payment option. | 2 | Consider favourites, recent contacts and a safe repeat-payment flow. Keep advanced options available without crowding the main dashboard. |
| **8** | **Aesthetic and minimalist design** | The minimal blue-and-white layout, whitespace and grouped cards create a clean visual direction. Too many banners, cards or decorative elements could weaken this simplicity. | 1 | Keep the home screen focused on essential payment tasks. Maintain readable contrast, consistent spacing and a clear visual hierarchy. |
| **9** | **Help users recognise, diagnose & recover from errors** | A failed or pending transaction needs a useful explanation. A generic error message may leave users unsure whether money was deducted or what to do next. | 3 | Use specific messages for failed, pending and network-error cases. Explain the next step and provide a transaction reference when available. |
| **10** | **Help and documentation** | The main payment shortcuts are intended to be self-explanatory, but users may still need help with payment status, bank linking or resolving a failed transaction. | 2 | Add a Help or Support entry in Profile and contextual help for payment issues. Include simple FAQs and a way to contact support in a real implementation. |
| **11** | **Accessibility** | Clear labels and spacing support readability, but accessibility cannot be confirmed from appearance alone. Colour contrast, text scaling and screen-reader labels need testing. | 2 | Check text/background contrast, use text labels in addition to colour, support larger text and add accessible names for icons and controls. |
| **12** | **Responsive & mobile-friendly layout** | MalhotraUPI is intended as a mobile-first payment interface. Its layout should remain usable on smaller screens and with different text sizes. | 2 | Test on multiple mobile screen sizes. Prevent clipped labels and overlapping cards, and ensure tap targets are comfortably sized. |
| **13** | **Privacy and trust cues** | A payment app handles sensitive financial information. A clean appearance alone does not establish security or explain how user data is handled. | 3 | Show only necessary account details, mask sensitive information where appropriate and provide clear privacy, security and transaction-confirmation information. |
| **14** | **Transaction history & information clarity** | A transaction list is useful only when users can quickly identify the recipient, amount, date and status. Missing or inconsistent details can make records difficult to understand. | 2 | Use a consistent transaction row with recipient, amount, date/time and status. Add filters or search if the history becomes long. |
| **15** | **Feedback and interaction responsiveness** | Buttons and screen transitions are intended to provide a responsive feel. Every important tap should produce visible feedback so users know it has been registered. | 2 | Add pressed states, loading indicators and confirmation feedback. Disable duplicate payment submission while a transaction is processing. |
| | **TOTAL SCORE** | **15 Heuristics Evaluated** | **29 / 75** | **Lower is better. Highest-priority issues identified: error prevention, error recovery, and privacy/trust cues.** |

---

## Part II: Other Observations (Beyond the Heuristics)

| S.No. | Observation | Comments / Recommendations |
| :---: | :--- | :--- |
| **1** | **Payment Safety & Confirmation** | A payment interface should make the recipient and amount easy to verify before the user confirms. A demo prototype should clearly indicate that it is not processing real money. |
| **2** | **UPI-Specific Edge Cases** | The design should account for incorrect UPI IDs, unavailable bank servers, insufficient balance, daily limits, duplicate taps and delayed transaction status. |
| **3** | **Empty and First-Time States** | A new user may have no linked bank account or transaction history. Empty states should explain what to do next instead of showing a blank screen. |
| **4** | **Network Interruptions** | The app should communicate when the network is unavailable and avoid encouraging users to retry a payment before checking its current status. |
| **5** | **Data Privacy** | Sensitive account information should not be exposed unnecessarily in screenshots, notifications or shared-device situations. |
| **6** | **User Testing** | Test the same tasks with several users: locate the QR scanner, send a demo payment and find a previous transaction. Record task success, time, errors and ease-of-use feedback. |

---

## Overall Conclusion
MalhotraUPI has a promising design direction for users who mainly need everyday UPI functions. Its focused dashboard, clear payment shortcuts and minimal visual style are intended to make common tasks easier to find. The most important areas to validate are payment error prevention, recovery from failed or pending transactions, accessibility, and privacy cues.
