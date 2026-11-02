# Experiment 7: Accessible Redesign of UPI Payment Experience (WCAG 2.2)

- **Student Name:** Nisarg Malhotra
- **Roll Number:** 29
- **PRN:** 1262243207
- **Class / Batch:** TY AI_DS Panel-F, Batch-F2
- **Date of Submission:** 02 November 2026
- **Project:** MalhotraUPI — Accessible Redesign of UPI Payment Experience
- **Figma Prototype Link:** [Figma Accessible Redesign v7](https://www.figma.com/proto/MalhotraUPI-Accessible-v7)

---

## 1. Aim
To redesign the interface of the MalhotraUPI application developed in previous lab assignments for users with special needs, and to create an accessible and inclusive interactive prototype compliant with WCAG 2.2 standards.

---

## 2. Problem Statement
Use the MalhotraUPI project and Figma prototype, redesign it for users with special needs (visual, motor, and cognitive impairments), apply accessibility guidelines (WCAG 2.2 Level AA), and check the final design against a comprehensive accessibility evaluation checklist.

---

## 3. Theoretical Framework
Accessible (inclusive) design means designing a product so that people with different abilities can use it effectively, efficiently, and with satisfaction. A limitation can be:
- **Permanent:** Blindness, profound deafness, severe motor tremors.
- **Temporary:** A sprained wrist, recovery from eye surgery.
- **Situational:** Bright outdoor sunlight, high stress during quick checkout counter transactions.

Designing for these edge constraints fundamentally improves usability for everyone. The Web Content Accessibility Guidelines (WCAG 2.2) serve as the foundation, structured around the four **POUR** principles:
1. **Perceivable:** Minimum text contrast ratio of $4.5:1$ for body copy and $3:1$ for essential graphical UI components; zero reliance on color alone to convey transaction status.
2. **Operable:** Minimum touch target sizes of $44 \times 44 \text{ px}$ (implemented as $48 \times 48 \text{ px}$); full keyboard/switch navigation with visible $3 \text{ px}$ focus indicators; non-gesture button alternatives for swipe-to-pay actions.
3. **Understandable:** Plain, consistent financial terminology, step-by-step single-focus task flows, and clear undo/cancel mechanisms.
4. **Robust:** Compatible with mobile assistive technologies including Android TalkBack, Apple VoiceOver, and external switch controls.

---

## 4. Problem Definition
The original MalhotraUPI prototype evaluated in Assignment 5 & 6 showed several usability barriers for users with accessibility needs:
1. **Low Contrast Labels:** Secondary text (timestamps, IFSC codes, micro-labels) had a contrast ratio of $3.1:1$, failing the WCAG AA requirement ($4.5:1$).
2. **Color-Only Status Indicators:** Payment success (green), pending (yellow), and failure (red) relied solely on colored dots without accompanying icon shapes or textual descriptors.
3. **Complex Touch Targets:** Action controls like "Cancel Payment" or "Remove Linked Account" had target heights under $30 \text{ px}$, causing frequent misclicks for users with motor tremors.
4. **Cognitive Overload during Confirmation:** Sending money displayed multiple inline prompts, popups, and small numerical fields simultaneously.
5. **No Undo Mechanism:** Accidentally triggering a payment or account removal could not be undone or easily reviewed.

---

## 5. Target User Groups
Students and everyday mobile payment users with mixed special needs:

| Group | Who | What They Need from MalhotraUPI |
| :--- | :--- | :--- |
| **Vision** | Low vision, red-green color blindness, users using 150–200% screen zoom | Text contrast $\ge 4.5:1$, payment status in distinct icons + words, high contrast mode, and dynamic screen reflow without breaking layout. |
| **Motor** | Tremors, one-handed users, temporary wrist injury, switch-access users | Large touch targets ($\ge 44 \text{ px}$), no swipe/drag-only approvals, full keyboard/switch accessibility with visible focus rings. |
| **Cognitive** | Dyslexia, ADHD, financial transaction anxiety, memory loss | One step per screen, plain financial language, clear confirmation screens with explicit "Undo / Cancel" timeouts. |

---

## 6. User Personas

| Feature | Meera Joshi, 21 (Vision) | Rohan Deshpande, 23 (Motor) | Sana Khan, 20 (Cognitive) |
| :--- | :--- | :--- | :--- |
| **Background** | B.Tech 3rd year. Low vision (175% zoom), red-green color blindness. | MBA 1st year. Tremor in right hand after a motorcycle injury. | BBA 2nd year. Dyslexia and high anxiety during financial tasks. |
| **Goal** | Scan QR codes and verify transaction success without squinting or guessing colors. | Send money to contacts cleanly without accidental wrong clicks. | Complete a UPI transaction clearly without confusing terminology or screen clutter. |
| **Frustrations** | Green/Red transaction status dots look identical; small gray timestamps fade out. | Tiny "Back" buttons and small keypads trigger misclicks; swipe-to-pay is hard. | Complex multi-banner dashboards cause distraction; small numeric pin inputs increase panic. |
| **Needs** | High contrast ($6.5:1+$), text labels alongside icons, high-contrast toggle. | Large buttons ($48 \text{ px}$), button-tap alternatives to swiping, clear focus outlines. | Single-focus transaction steps, standard plain terms ("Pay", "Sent"), clear transaction summary. |

---

## 7. Redesigned Screen Flow
The core UPI payment journey was redesigned to ensure every step is operable via touch, high-contrast display, or switch controls:
- **Step A1 (Home Dashboard):** Clean primary bar, accessible scan shortcut, high-contrast toggle.
- **Step A2 (Send Money - Select Contact):** High-contrast contacts list, large tap targets ($52 \text{ px}$ contact rows).
- **Step A3 (Enter Amount & Note):** Clean numeric entry with large 28px bold legible text and explicit primary focus.
- **Step A4 (Payment Confirmation & Review):** Step-by-step modal showing exact recipient, bank, and amount with explicit "Confirm Pay" and "Cancel" buttons (no drag required).
- **Step A5 (Transaction Success / Status Screen):** Distinct icon shape (Checkmark inside Shield), explicit text ("Payment Successful"), announced screen-reader alert, and optional "Undo Recipient Save".

---

## 8. Redesigned Screens & Accessibility Improvements

| Screen | Change Implemented | Target Group | WCAG Guideline |
| :--- | :--- | :--- | :--- |
| **A1 Home Dashboard** | Simplified dashboard with single primary "Scan QR" and "Send Money" actions; text size increased to 16px minimum. | Cognitive, Vision | **1.4.3 Contrast; 3.2.3 Consistency** |
| **A1 Home Dashboard** | "Display & Accessibility" settings modal added to top bar (High Contrast, Large Font, Reduce Motion). | Vision, Motor | **1.4.4 Resize Text; 2.3.3 Motion** |
| **A2 Contact Selection** | Increased contact row height to $52 \text{ px}$; added visible blue $3 \text{ px}$ focus indicator for keyboard/switch navigation. | Motor | **2.5.8 Target Size; 2.4.7 Focus Visible** |
| **A3 Enter Amount** | Number font size scaled to 28px bold; currency symbol labeled clearly in text (`INR (₹)`). | Vision, Cognitive | **1.4.3 Contrast; 3.3.2 Labels** |
| **A4 Payment Review** | Removed swipe-to-pay slider; replaced with dual high-contrast action buttons: "Confirm & Pay" ($48 \text{ px}$) and "Cancel". | Motor, Cognitive | **2.5.7 Dragging Movements; 3.3.4 Error Prevention** |
| **A5 Transaction Details** | Status indicated by text ("SUCCESSFUL"), icon (Shield Check), and color (Dark Teal). Urgent/Failed states use Warning Triangles. | Vision | **1.4.1 Use of Color** |
| **All Screens** | Text contrast raised to $6.6:1$; interactive border contrast raised to $4.2:1$; focus ring contrast $6.7:1$. | Vision, Motor | **1.4.3 Contrast; 1.4.11 Non-Text Contrast** |

---

## 9. Accessibility Checklist Verification (WCAG 2.2 Level AA)

| Check | WCAG 2.2 | Result | How MalhotraUPI Meets It |
| :--- | :---: | :---: | :--- |
| **Text contrast $\ge 4.5:1$** | 1.4.3 AA | **Pass** | Primary body text $12.1:1$, secondary details $6.6:1$, button labels $6.3:1$. |
| **Controls contrast $\ge 3:1$** | 1.4.11 AA | **Pass** | Input fields and button outlines have $4.2:1$ contrast against background. |
| **Color is not the only cue** | 1.4.1 A | **Pass** | Success uses Checkmark+Shield; Failure uses Cross+Triangle; text states explicitly written. |
| **Text can be enlarged** | 1.4.4 AA | **Pass** | Dedicated font-scaling setting inside the app (Default, Large, Extra Large). |
| **Target size $\ge 44 \text{ px}$** | 2.5.8 AA | **Pass** | All payment action buttons are $48 \text{ px}$ high with $12 \text{ px}$ padding. |
| **Alternative to dragging** | 2.5.7 AA | **Pass** | Swipe-to-confirm replaced with direct button tap or Enter key. |
| **Keyboard/Switch operable** | 2.1.1 A | **Pass** | Full tab sequence configured across all Figma prototype screens. |
| **Focus visible** | 2.4.7 AA | **Pass** | Solid $3 \text{ px}$ deep blue ring visible around active focused UI element. |
| **Labels & instructions** | 3.3.2 A | **Pass** | Clear field labels ("Recipient UPI ID", "Amount in ₹") above every input. |
| **Error prevention / Undo** | 3.3.4 AA | **Pass** | Explicit confirmation screen prior to PIN entry; quick cancel button available. |
| **Status messages announced** | 4.1.3 AA | **Pass** | Success screen formatted as ARIA live region status container. |
| **Consistent navigation** | 3.2.3 AA | **Pass** | Top navigation bar and primary bottom navigation remain identical across views. |

---

## 10. Evaluation & Simulation Testing Summary
1. **Color Blindness Simulation (Deuteranopia & Protanopia):**  
   *Finding:* Success (green) and Pending (amber) badges were distinguishable by hue, but text labels ("SUCCESS", "PENDING") and icon shapes (Checkmark vs. Hourglass) ensured 100% clarity regardless of vision type.
2. **Low Vision (Blur & Contrast Filter):**  
   *Finding:* Primary payment buttons and transaction amounts remained legible at blur levels up to 3px due to large typography ($24\text{px}+$) and strong background contrast ($6.6:1$).
3. **Keyboard & Switch Navigation Walkthrough:**  
   *Finding:* A complete payment simulation (Select Contact $\rightarrow$ Enter Amount $\rightarrow$ Confirm $\rightarrow$ Success) was executed using only Tab, Spacebar, and Enter keys. Focus indicators moved predictably through every interactive control.

---

## 11. Conclusion
In this assignment, the MalhotraUPI mobile payment application was redesigned to meet WCAG 2.2 Level AA accessibility standards. By resolving high-contrast deficits, eliminating reliance on color-only status indicators, removing gesture-only interaction patterns (such as swiping to pay), increasing touch target sizes to $48\text{px}$, and introducing a dedicated Display & Accessibility settings menu, MalhotraUPI ensures that users with visual, motor, and cognitive impairments can conduct digital financial transactions safely and independently.

---

## 12. Frequently Asked Questions (FAQs)

### 1. Explain the four principles of WCAG (POUR) with suitable examples.
- **Perceivable:** Information must be presentable to users in ways they can perceive. *Example:* Text contrast of at least $4.5:1$ and providing textual/iconic alternatives for transaction status colors.
- **Operable:** Interface components must be operable with various input methods. *Example:* Ensuring every payment button can be activated via keyboard/switch access without requiring drag gestures.
- **Understandable:** Information and operation must be clear. *Example:* Using plain financial language ("Send Money", "Bank Account") and providing clear transaction confirmation screens.
- **Robust:** Content must be compatible with current and future assistive technologies. *Example:* Using proper screen reader labels and ARIA status announcements for payment completion messages.

### 2. Discuss design considerations for users with visual, hearing, motor, and cognitive impairments in financial apps.
- **Visual:** High contrast ratios, resizable font options, non-color status cues, screen reader compatibility.
- **Hearing:** Visual notification banners and haptic feedback instead of sound-only transaction chimes.
- **Motor:** Touch targets $\ge 44\text{px}$, well-spaced layout elements, no precise drag/swipe gestures required for payment authorization.
- **Cognitive:** Step-by-step transaction wizard, minimal dashboard clutter, explicit confirmation steps, and clear undo/cancel controls.
