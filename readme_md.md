# ScamShield AI - Online Scam Detection Chatbot

**Course:** Artificial Intelligence: Real-World Applications and Implications  
**Student Name:** Sayar Patel  
**School:** Ryan Global School, Kharghar  
**Program:** IBCP Year 1  

## 🌐 Live Chatbot Link
**Try ScamShield AI here:** [Live Web Demo](https://bot.dialogflow.com/2e1754e8-b2fb-4e04-8173-4f2c62960471)

---

## 📖 Project Overview
In today's digital age, everyday users rely heavily on mobile phones for payments, shopping, and job hunting. Unfortunately, this has led to a rise in digital fraud, such as fake UPI requests, phishing links, and deceptive job offers. 

**ScamShield AI** is an intelligent, conversational digital safety assistant built using Google Dialogflow. Its primary goal is to help users—specifically students, the elderly, and job seekers—verify whether a message, call, or offer is a scam. By providing clear, cautionary, and easy-to-understand advice, ScamShield AI educates users on online safety and helps them make secure decisions in real-time.

---

## 🧠 Intents and Entities

The chatbot uses Natural Language Understanding (NLU) powered by Google Dialogflow. It is trained using 15 distinct intents and 10 custom entities to accurately understand and extract information from user queries.

### Custom Entities (10)
Entities allow the chatbot to extract specific data points from the user's input.
1. **`@ScamType`**: Identifies the category of fraud (e.g., *upi, phishing, job scam, otp*).
2. **`@UrgencyLevel`**: Detects pressure tactics used by scammers (e.g., *high, immediate, urgent*).
3. **`@PaymentApp`**: Recognizes popular financial platforms (e.g., *googlepay, phonepe, paytm*).
4. **`@FinancialAction`**: Captures the user's action (e.g., *paid, clicked, shared, downloaded*).
5. **`@CommunicationChannel`**: Identifies how the scam was received (e.g., *sms, whatsapp, phonecall*).
6. **`@TargetInfo`**: Recognizes sensitive data targeted by scammers (e.g., *otp, password, aadhaar, pan*).
7. **`@EmploymentType`**: Detects job-related keywords (e.g., *workfromhome, dataentry*).
8. **`@InvestmentType`**: Identifies investment vehicles often used in scams (e.g., *crypto, stocks, scheme*).
9. **`@RiskIndicator`**: Flags common scam bait tactics (e.g., *upfrontfee, freegift*).
10. **`@FeedbackRating`**: Captures user satisfaction (e.g., *helpful, unhelpful*).

### Intents (15)
Intents map what a user says to the appropriate chatbot response. 
1. **`Default Welcome Intent`**: Greets the user and introduces ScamShield AI.
2. **`ScamCheckIntent`**: Prompts the user to share the suspicious message they received.
3. **`OTPIntent`**: Warns users never to share their OTP, PIN, or passwords.
4. **`UPIFraudIntent`**: Educates users on UPI "collect requests" and fake payment notifications.
5. **`JobOfferFraudIntent`**: Helps users spot fake work-from-home offers and upfront fee scams.
6. **`PhishingLinkIntent`**: Advises users on handling unknown links and immediate disconnection if clicked.
7. **`InvestmentScamIntent`**: Warns against guaranteed high-profit returns and money-doubling schemes.
8. **`LoanFraudIntent`**: Identifies fake instant loan apps and advance fee traps.
9. **`KYCUpdateIntent`**: Alerts users about fake bank or SIM block threats tied to KYC updates.
10. **`LotteryPrizeIntent`**: Warns users about fake prize claims requiring initial tax/fee payments.
11. **`ReportFraudIntent`**: Provides official government cybercrime reporting portals and helpline numbers (e.g., 1930).
12. **`SafetyTipsIntent`**: Shares best practices for general digital hygiene and security.
13. **`AwarenessQuizIntent`**: Engages users with interactive True/False questions about digital safety.
14. **`FallbackIntent`**: Gracefully handles unrecognized user inputs and redirects the conversation.
15. **`GoodByeIntent`**: Ends the chat warmly and encourages the user to stay alert.

---

## ⚙️ Integration Details
This chatbot is built using **Google Dialogflow ES (Essentials)**. 
* It handles conversational logic, context management, and slot-filling directly within the Dialogflow console.
* The current deployment utilizes Dialogflow's native **Web Demo** integration, which provides a lightweight, shareable iframe/URL for instant public access without requiring a custom frontend.

---

## 🚀 Deployment Instructions

If you wish to deploy this agent into your own Google Dialogflow account, follow these steps:

1. **Download the Agent Files:**
   Clone or download this repository to your local machine. Ensure you have the agent `.zip` file (which contains the `agent.json`, `package.json`, `intents/`, and `entities/` folders).
2. **Create a New Agent in Dialogflow:**
   * Go to the [Dialogflow ES Console](https://dialogflow.cloud.google.com/).
   * Click **Create Agent** in the left menu.
   * Give the agent a name (e.g., `ScamShield-Copy`), select your default language and timezone, and click **Create**.
3. **Import the Project:**
   * Click the **Gear icon (Settings)** next to your agent's name.
   * Go to the **Export and Import** tab.
   * Select **Restore from ZIP**.
   * Upload the provided `.zip` file from this repository and type `RESTORE` in the text box to confirm.
   * Click **Restore**.
4. **Enable Web Integration:**
   * Navigate to the **Integrations** tab in the left sidebar.
   * Enable the **Web Demo** toggle.
   * Click on the Web Demo link to get your live shareable URL.