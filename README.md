This repository contains a fully automated **email outreach system** designed to efficiently send **personalized emails at scale** and process responses. The project leverages Python’s **SMTP** and **IMAP** libraries to manage influencer outreach, track responses, and handle follow-ups.  

---

## **Features**  
✅ **Automated Email Sending** – Sends personalized emails to influencers from multiple sender accounts.  
✅ **Spam Prevention** – Uses sender rotation and randomized delays to prevent emails from being flagged as spam.  
✅ **Inbox Monitoring & Reply Handling** – Automatically fetches replies and extracts relevant details.  
✅ **Follow-Up Automation** – Sends targeted follow-up emails to engaged users.  
✅ **Scalability & Efficiency** – Designed to handle large volumes of emails while maintaining personalization.  

---

## **Tech Stack**  
- **Python** – Core programming language  
- **pandas** – Handling influencer data stored in Excel  
- **smtplib, email** – Sending automated emails  
- **imaplib** – Fetching and processing email responses  
- **re (Regex)** – Extracting relevant details (e.g., phone numbers) from responses  

---

## **How It Works**  

### **1️⃣ Sending Automated Emails**  
- Loads influencer data from an **Excel sheet**.  
- Dynamically personalizes email content for each recipient.  
- Sends emails using multiple sender accounts in a **rotating** manner.  
- Introduces a **random delay** between emails to avoid spam detection.  

### **2️⃣ Handling Replies & Extracting Data**  
- Monitors **inbox responses** using IMAP.  
- Extracts **contact details** (e.g., phone numbers) from replies.  
- Updates an **Excel database** with collected data for further processing.  

### **3️⃣ Sending Follow-Up Emails**  
- Identifies recipients who have responded.  
- Sends **customized follow-up emails** based on previous interactions.  
- Ensures continuity in communication for improved engagement.  

---

## **Setup & Usage**  

### **🔧 Installation**  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/email-outreach-automation.git
   cd email-outreach-automation
   ```
2. Install dependencies:  
   ```bash
   pip install pandas openpyxl
   ```
3. Replace placeholders with actual **email credentials** (**Use environment variables for security**).  
4. Update **Excel file paths** with your dataset.  
5. Run the script:  
   ```bash
   python email_automation.py
   ```

---

## **Security & Best Practices**  
⚠️ **DO NOT store email credentials in the script.** Use environment variables instead.  
⚠️ Ensure compliance with **email sending policies** to avoid blacklisting.  
⚠️ Use **dedicated email accounts** for outreach to prevent your primary accounts from being flagged.  

---
