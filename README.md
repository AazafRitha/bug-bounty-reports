# Bug Bounty & Vulnerability Research Reports (2024–2025)

This repository contains a collection of **10 vulnerability assessment reports** documenting real-world web security issues.  
Each report follows **OWASP Top 10 methodology** and includes **impact assessment, reproduction steps, proof of concept (PoC), and remediation recommendations**.  

---

## 📂 Reports Included

1. **Cryptographic Failures – gov.lk**  
   Weak SSL/TLS configuration (TLS 1.0/1.1, weak DH params, AES-CBC, NULL compression).  
   *Tools:* Nmap, testssl.sh, SSL Labs  

2. **PII Exposure & Reflected XSS – ranjanlanka.lk**  
   Personal data leakage in URLs and reflected XSS via query parameters.  
   *Tools:* Burp Suite, OWASP ZAP, XSStrike  

3. **Clickjacking – meatmart.lk**  
   Lack of X-Frame-Options / CSP headers → iframe-based attack surface.  
   *Tools:* Nikto, OWASP ZAP  

4. **Open Redirect – rainbowpages.lk**  
   Vulnerable redirect endpoint (`/out.php`) enabled phishing and credential theft.  
   *Tools:* Burp Suite, OWASP ZAP  

5. **CORS Misconfiguration – ido.lk**  
   Insecure CORS policy (`Access-Control-Allow-Origin: *`) allowed cross-origin attacks.  
   *Tools:* OWASP ZAP, Browser DevTools  

6. **Vulnerable JS Library – Truecaller**  
   Outdated `moment.js v2.22.2` with CVEs enabling prototype pollution & XSS.  
   *Tools:* OWASP ZAP, Burp Suite  

7. **Vulnerable JS + PII Exposure – Greenfly**  
   Outdated `pdf.js` library (CVE-2024-4367) and exposed credit card data.  
   *Tools:* OWASP ZAP, curl  

8. **Missing CSP Header – Mergify**  
   Absence of CSP header → exposed to XSS and clickjacking risks.  
   *Tools:* Nikto, OWASP ZAP  

9. **Hash Disclosure – Neon.tech**  
   Publicly exposed BCrypt hash in frontend HTML response.  
   *Tools:* OWASP ZAP, Browser DevTools  

10. **PII Disclosure – KHealth**  
    Raw credit card number leaked in HTTP response body.  
    *Tools:* Burp Suite, OWASP ZAP  

---

## 🛠️ Tools & Methodologies
- **Tools:** Burp Suite, OWASP ZAP, Nikto, Nmap, testssl.sh, Subfinder  
- **Methodologies:** OWASP Top 10, Manual Testing, Proof of Concept (PoC), Responsible Disclosure Practices  

---

## ⚖️ Disclaimer
These reports were created for **academic, ethical testing, and bug bounty learning purposes only**.  
No unauthorized exploitation was performed.  

---

## 👤 Author
**Aazaf Ritha J**  
- 🎓 Cybersecurity Undergraduate @ SLIIT  
- 🌐 [LinkedIn](https://linkedin.com/in/aazafritha)  
- 💻 [GitHub](https://github.com/aazafritha)  
