# 🛡️ Phishing Email Threat Analysis  
**Internship Task 2 – Network Security**

---
## 📚 Table of Contents

- [Objective](#objective)
- [Tools Used](#tools-used)
- [Repository Structure](#repository-structure)
- [Sample Analyzed](#sample-analyzed)
- [Header Analysis Summary](#header-analysis-summary)
- [Phishing Indicators Found](#phishing-indicators-found)
- [Key takeaways](#key-takeaways)
- [Author](#author)

  ---
  
## 🎯 Objective  
To analyze a phishing email sample, identify spoofing techniques, and understand how attackers manipulate email headers and language to deceive users.

---

## 🧰 Tools Used

- 📧 **Gmail** – to view and copy raw email headers  
- 🔎 **[MXToolbox Email Header Analyzer](https://mxtoolbox.com/EmailHeaders.aspx)** – to analyze email headers  
- 🌐 **Web browser** – to hover over links and verify mismatches

  ---

  ## 📂 Repository Structure

| File | Description |
|------|-------------|
| `phishing-report.md` | Full analysis report (markdown file) |
| `README.md` | Project overview (this file) |
| *(Optional)* screenshots / email sample |

---

## 📬 Sample Analyzed 

- **Subject:** _Important: Your PayPal account is on hold_  
- **Sender Email:** `support@paypa1.com`  
- **Fake Link (shown):** `https://paypal.com/verify`  
- **Actual Link (real):** `http://malicious-verify-paypal.com/login`  
- **Tone:** Urgent and threatening  

---

## 🧪 Header Analysis Summary  
Using MXToolbox:

| Check         | Status   |
|---------------|----------|
| SPF           | ❌ Failed |
| DKIM          | ❌ Failed |
| DMARC         | ❌ Failed |
| IP Address    | `185.174.149.16` |
| Sending Domain | `mail.paypa1.com` (not genuine) |

---

## 🚩 Phishing Indicators Found

- ✉️ **Spoofed sender address** (looks like PayPal but isn’t)  
- 🔗 **Misleading links** – real destination different from what’s shown  
- 📛 **Spelling & grammar errors** – typical of phishing scams  
- ⚠️ **Urgent, threatening tone** – to trigger panic  
- ❌ **Failed SPF/DKIM/DMARC** – failed security checks  
- 🌍 **Unverified source IP address**

---

## 💡 Key Takeaways

- Always **check sender email** carefully  
- Use **header analysis tools** to validate legitimacy  
- Watch out for **urgent or fear-based messages**  
- **Hover over links** before clicking  
- Understand how **SPF, DKIM, and DMARC** help protect against spoofing

---

## 👩‍💻 Author

**Swaranjali** 
**Cybersecurity Intern | Electronics and Communication Engineering Student** 
[GitHub Profile](https://github.com/swaranjali-ops)
