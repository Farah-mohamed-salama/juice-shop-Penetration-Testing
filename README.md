# OWASP Juice Shop

## Executive Summary
I conducted a comprehensive penetration test to evaluate the security posture of the **OWASP Juice Shop** web application. This assessment aimed to identify and exploit vulnerabilities in the configuration and implementation of the Juice Shop service. The penetration test simulated the actions of an external threat actor attempting to compromise various systems by exploiting multiple vulnerabilities within the service.

### Demo Website
- Explore the application: [OWASP Juice Shop Demo](https://demo.owasp-juice.shop/#/)
- Learn more about the OWASP Juice Shop Project: [OWASP Juice Shop Project](https://owasp.org/www-project-juice-shop/)

---

## Test Scope and Method
The test focused on evaluating the security of the Juice Shop application, which is intentionally designed with vulnerabilities for educational and testing purposes. The methodology included manual penetration testing techniques combined with automated tools to uncover security flaws.

---

## Overall Risk Rating
The overall risk rating for the Juice Shop application is **High**, as the identified vulnerabilities expose the application to potential exploitation, leading to data breaches, privilege escalation, and manipulation of sensitive information.

---

## Found Vulnerabilities
The following vulnerabilities were identified during the assessment:

1. **SQL Injection (Login Admin):** Exploiting SQL injection on the login form to gain administrative access.  
   - **Impact:** Unauthorized access to admin functionalities.

2. **Unauthorized Privilege Escalation:** Escalating user privileges to access administrative features.  
   - **Impact:** Full control of restricted operations.

3. **API-only Cross-Site Scripting (XSS):** Injecting malicious scripts via API endpoints.  
   - **Impact:** Potential account compromise or data theft.

4. **Broken Access Control:** Bypassing restrictions to perform unauthorized actions.  
   - **Impact:** Exposing sensitive user data and functionality.

5. **Unauthorized Modification of Data:** Altering another user's data through insecure endpoints.  
   - **Impact:** Data integrity violations.

6. **Unauthorized Viewing of Another User's Basket:** Gaining access to other users’ shopping baskets.  
   - **Impact:** Breach of user confidentiality.

7. **Unauthorized Deletion of Items in Another User's Basket:** Deleting items from another user's shopping basket without permission.  
   - **Impact:** Loss of user data and potential disruption of their experience.

8. **Sensitive Information Exposure:** Leakage of sensitive information like API keys and credentials.  
   - **Impact:** Increased attack surface for threat actors.

9. **DOM-Based Cross-Site Scripting (XSS) via Search Bar:** Injecting scripts through the search bar.  
   - **Impact:** Client-side attacks, including data theft and session hijacking.

---

## Technical Explanation
Each identified vulnerability demonstrates real-world attack scenarios that are commonly exploited in web applications. This project serves as a learning platform for understanding the impact of insecure coding practices.

---

## Conclusion
This penetration test revealed multiple critical vulnerabilities in the Juice Shop application, showcasing the importance of secure development practices. Developers and security professionals should address these issues to enhance the application's security posture.

To experiment with these vulnerabilities in a controlled environment, visit the demo: [OWASP Juice Shop Demo](https://demo.owasp-juice.shop/#/).

---

## Disclaimer
This assessment was conducted in a controlled environment for educational purposes. Testing applications without proper authorization is illegal and unethical.
