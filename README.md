# ElevateLabs_CS_Task02
Analyze a Phishing Email Sample
# Task 2: Analyze a Phishing Email Sample

## 🎯 Objective
Identify phishing characteristics in a suspicious email by analyzing headers, sender details, links, and content.

---

## 🛠️ Tools Used
- Saved phishing email (`sample_phishing.eml`)
- Online Email Header Analyzer (e.g., MXToolbox, Google Header Analyzer)
- Text editor (to open raw email file)

---

## 📖 Steps Taken
1. **Obtained a phishing email sample** in `.eml` format.
2. **Examined sender address** — found mismatches between display name and actual domain.
3. **Analyzed headers** using an online header analyzer:
   - Checked SPF, DKIM, DMARC results.
   - Reviewed `Received:` paths to trace origin.
4. **Inspected links and attachments**:
   - Hovered links showed mismatched domains.
   - Noted presence of suspicious file attachments.
5. **Reviewed email body**:
   - Found urgent language (“Verify now”, “Your account will be closed”).
   - Identified poor grammar and spelling errors.
6. **Summarized findings** in a phishing report with screenshots.

---

## 📊 Findings
- **Spoofed sender domain** not matching real company.
- **Failed SPF/DKIM authentication** in headers.
- **Mismatched URLs** (e.g., showed `paypal.com` but linked to `bit.ly/...`).
- **Suspicious attachment** (`invoice.docm`) likely containing macros.
- **Urgent + threatening tone** to pressure the victim.
- **Grammar mistakes** common in phishing attempts.

---

## 📂 Repository Contents
- `sample_phishing.eml` – Sample phishing email (safe text file, sanitized).
- `reports/phishing_analysis.md` – Detailed phishing indicators found.
- `screenshots/` – Evidence (header analyzer results, email body, URL hover test).
- `README.md` – This documentation file.

---

## ✅ Key Learnings
- Email headers reveal spoofing and authentication failures.
- Hovering over links is a simple but effective way to catch mismatched URLs.
- Social engineering tactics (urgency, threats) are key phishing indicators.
- Attachments with executable content or macros are a major red flag.

---

## ▶️ How to Reproduce
1. Save any phishing email in `.eml` format.
2. Open the raw headers and paste them into an **email header analyzer**.
3. Compare sender details and check authentication results.
4. Extract and review URLs and attachments.
5. Write a short phishing report summarizing suspicious traits.
