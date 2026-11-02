# Experiment 2: Personas and User Journey Mapping

- **Student Name:** Nisarg Malhotra
- **Roll Number:** 29
- **PRN:** 1262243207
- **Class / Batch:** TY AI_DS Panel-F, Batch-F2
- **Domain:** UPI Payment Apps (Google Pay, PhonePe, Paytm)

---

## 1. Empathy Map: Everyday UPI Payment App Users

| Quadrant | User Behaviors & Expressions |
| :--- | :--- |
| **SAYS** | <ul><li>"Did you receive the money?"</li><li>"Why did the layout change again?"</li><li>"Scan my code, my camera isn't working."</li><li>"It says processing, should I pay again?"</li></ul> |
| **THINKS** | <ul><li>Wonders if their money is safe when the network drops mid-transaction.</li><li>Believes the app assumes everyone knows how to read English fluently.</li><li>Worries that a slightly different UI means they clicked a spam link.</li></ul> |
| **DOES** | <ul><li>Double-checks the receiver's name out loud before entering the UPI PIN.</li><li>Relies completely on the merchant's soundbox for payment confirmation.</li><li>Sticks strictly to the "Scan QR" button and ignores all other features.</li></ul> |
| **FEELS** | <ul><li>Anxious about typing the wrong PIN in a crowded space.</li><li>Relieved the moment they hear the confirmation chime.</li><li>Frustrated and overwhelmed by pop-up ads and dense mini-app menus.</li></ul> |

---

## 2. Four Core User Pain Points in Modern UPI Interfaces

1. **Clutter Obscures Core Actions:**  
   Users open the app simply to pay, but are bombarded with loans, games, and ads. The core action gets buried, leading to cognitive overload.
2. **Layout Instability:**  
   Constant UI updates completely break the spatial memory of semi-literate users who rely heavily on muscle memory to navigate the app.
3. **Ambiguous Error States:**  
   When a payment says "Processing", users panic. Unclear guidance leads them to hit 'pay' again, resulting in stressful duplicate transactions.
4. **Over-reliance on Text:**  
   Critical financial alerts rely on tiny English text rather than universally understood visual cues or color codes, alienating non-fluent users.

---

## 3. User Personas

### Persona 1: Raju Sharma
- **Profile:** Street Food Vendor
- **Location:** Pune, India
- **Platform Use:** PhonePe Merchant
- **Quote:** *"Just scan the code and show me the green tick, I am busy."*
- **Goals:**
  - Instant, undeniable confirmation that a payment was received.
  - An interface that requires zero reading during peak rush hours.
  - Clear, loud audio cues via the smart speaker (Soundbox).
- **Frustrations:**
  - Customers showing fake screenshot confirmations.
  - Network drops causing the speaker to delay its announcement.
  - Small text on the phone screen that is hard to read in bright sunlight.

### Persona 2: Sunita Patel
- **Profile:** Tech-Anxious Homemaker
- **Location:** Pune, India
- **Platform Use:** Google Pay
- **Quote:** *"I always double-check the phone number with my son before pressing send."*
- **Goals:**
  - Absolute confidence that her money is going to the correct person.
  - A simple, unchanging interface that she can memorize visually.
  - Easy access to recurring payments like electricity and dish TV.
- **Frustrations:**
  - Too many unfamiliar buttons on the screen make her nervous.
  - Fear of accidentally clicking the wrong thing and losing her money.
  - Error messages that use confusing technical banking terms.

### Persona 3: Aditi Desai
- **Profile:** Tech-Savvy Student
- **Location:** Pune, India
- **Platform Use:** GPay & PhonePe
- **Quote:** *"I use GPay for friends and PhonePe for stores, whichever opens faster."*
- **Goals:**
  - A lightning-fast way to scan, pay, and get out of the checkout line.
  - Seamless tools to split dinner bills and cab fares with friends.
  - An easy way to track monthly allowance and spending habits.
- **Frustrations:**
  - Apps that take too long to load due to heavy promotional graphics.
  - Having to manually calculate splits outside of the payment app.
  - Awkwardly waiting to ensure a friend received a transferred amount.

### Persona 4: Vikram Singh
- **Profile:** Small Business Owner
- **Location:** Pune, India
- **Platform Use:** Paytm for Business
- **Quote:** *"I need to know my end-of-day settlement without digging through menus."*
- **Goals:**
  - A clear, accessible daily ledger to match with physical cash registers.
  - Instant settlements directly to his connected bank account.
  - One-click tools for initiating customer refunds securely.
- **Frustrations:**
  - Business dashboards cluttered with unrelated consumer loan ads.
  - Hidden transaction fees for certain types of credit card scans.
  - Delayed settlements that disrupt cash flow for the next day.

### Persona 5: Rahul Kumar
- **Profile:** Migrant Blue-Collar Worker
- **Location:** Pune, India
- **Platform Use:** PhonePe
- **Quote:** *"I just want to send money to my village without the app hanging."*
- **Goals:**
  - An app that works flawlessly on a budget smartphone with 3G speeds.
  - A simple, visual interface that supports regional languages (Hindi).
  - Clear feedback if a transaction is pending or failed.
- **Frustrations:**
  - Heavy animations causing the app to freeze mid-transaction.
  - Error prompts displayed entirely in technical English.
  - Fear of losing a day's wages to a glitchy server timeout.

---

## 4. User Journey Maps

### Journey 1: Raju (Street Food Vendor) — Rush Hour Peak
- **Action:** Handling peak rush hour at the stall $\rightarrow$ Customer scans QR code $\rightarrow$ Waiting for confirmation $\rightarrow$ Moving quickly to the next customer.
- **Task List:** Hands over food package $\rightarrow$ Points to printed QR code $\rightarrow$ Listens for speaker announcement $\rightarrow$ Interrupts workflow to check phone screen if speaker fails.
- **Feeling:** Rushed and highly focused $\rightarrow$ Anxious when there is network lag $\rightarrow$ Relieved instantly by audio confirmation.
- **UX Opportunity:** Implement a full-screen visual flash (Bright Green/Red) on the phone screen allowing verification from a distance without reading text.

### Journey 2: Sunita (Homemaker) — Paying Electricity Bill
- **Action:** Decides to pay monthly electricity bill $\rightarrow$ Enters complex consumer number $\rightarrow$ Types secret UPI PIN $\rightarrow$ Encounters "Processing" screen.
- **Task List:** Opens app and navigates to 'Bills' $\rightarrow$ Types 12-digit number carefully $\rightarrow$ Asks family member to verify name $\rightarrow$ Presses pay and waits.
- **Feeling:** Nervous about making typos $\rightarrow$ Cautious before pressing confirm $\rightarrow$ Confused and scared if screen hangs on processing.
- **UX Opportunity:** Auto-fetch connected household billers via registered mobile number to eliminate manual data entry fear.

### Journey 3: Aditi (College Student) — Splitting Dinner Bill
- **Action:** Finishes dinner with friends $\rightarrow$ Calculating who owes what $\rightarrow$ Sending out payment requests $\rightarrow$ Tracking who has paid back.
- **Task List:** Pays total bill at restaurant $\rightarrow$ Opens calculator to divide total $\rightarrow$ Opens UPI app to manually send requests $\rightarrow$ Checks app daily for pending requests.
- **Feeling:** Generous covering bill $\rightarrow$ Annoyed by manual math and app switching $\rightarrow$ Frustrated reminding friends to pay.
- **UX Opportunity:** Built-in automated bill-splitting workflow popping up directly on the transaction success screen.

### Journey 4: Vikram (Shopkeeper) — Night Settlement
- **Action:** Closing shop late at night $\rightarrow$ Tallying day's digital payments $\rightarrow$ Checking bank settlement status $\rightarrow$ Locking up and going home.
- **Task List:** Opens Merchant app $\rightarrow$ Navigates past promotional loan banners $\rightarrow$ Finds daily total and compares with physical cash register.
- **Feeling:** Exhausted after a long day $\rightarrow$ Focused on verifying numbers $\rightarrow$ Satisfied once settlement is confirmed.
- **UX Opportunity:** A clean, ad-free merchant dashboard opening directly to the day's settlement ledger.

### Journey 5: Rahul (Migrant Worker) — Remittance Home
- **Action:** Receives monthly wages $\rightarrow$ Opens app on weak connection $\rightarrow$ Selects family contact $\rightarrow$ Initiates transfer.
- **Task List:** Opens app and waits for heavy UI $\rightarrow$ Scrolls to find saved contact $\rightarrow$ Enters amount and PIN $\rightarrow$ Prays connection holds.
- **Feeling:** Happy sending support home $\rightarrow$ Tense during slow loading animations $\rightarrow$ Relieved when green success tick appears.
- **UX Opportunity:** Introduce a 'Lite' mode that disables heavy animations for budget devices and low-bandwidth connections.
