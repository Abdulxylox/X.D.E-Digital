# Capstone Project: Cybersecurity Assessment and Hardening of X.D.E Digital Web Application

## 1. Introduction

This project evaluates and strengthens the security posture of the X.D.E Digital web application—a fintech platform designed for digital transactions. The aim is to identify vulnerabilities, apply threat modeling, and implement security controls to protect user data and financial operations.

## 2. Threat Modeling

Using the STRIDE framework, we identified key assets (user profiles, transaction data), potential threat actors (malicious users, external attackers), and risks such as spoofing, tampering, and information disclosure.

## 3. Security Assessment

The assessment revealed critical gaps: no backend authentication, hard-coded financial values, and no server-side authorization. Without these controls, the app is exposed to impersonation, tampering, and unauthorized access.

## 4. Security Controls Implemented

To mitigate these risks, we introduced a secure backend using Node.js and Express. User authentication is now handled via JWT, with passwords securely hashed using bcrypt. Role-based access controls ensure users only perform authorized actions. Input validation and security headers (CSP, HSTS) were added to protect against injection and other web vulnerabilities.

## 5. Testing and Validation

We tested authentication with both valid and invalid credentials, ensuring unauthorized access was blocked. Rate limiting prevented brute-force attempts. Input validation tests confirmed that malicious input was blocked. Security headers were validated using browser developer tools.

## 6. Conclusion

This project improved the security of X.D.E Digital by introducing a backend, robust authentication, and input validation. The risk of unauthorized access, data tampering, and information exposure was significantly reduced. Future work includes deploying a full production backend and integrating real-time transaction processing.
