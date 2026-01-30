# Cyber Security Internship – Task 4  
## Password Security & Authentication Analysis

---

## Task Objective

The objective of this task was to understand how password security works in real-world systems, why passwords are not stored in plain text, how hashing protects credentials, and how weak passwords can be cracked using common attack techniques. This task focused on learning the fundamentals of password security and authentication mechanisms from a defensive cyber security perspective.

---

## Scope of the Task

This task was strictly educational and did not involve attacking real systems or accounts. All experiments were performed using self-created test passwords in a controlled environment.

---

## Concepts Covered

- Password storage mechanisms  
- Hashing vs encryption  
- Common hashing algorithms  
- Weak vs strong password analysis  
- Dictionary and brute-force attacks  
- Practical hash cracking using Hashcat  
- Importance of Multi-Factor Authentication (MFA)  
- Password security best practices  

---

## Tasks Performed

### 1. Understanding How Passwords Are Stored
- Studied how websites do not store passwords in plain text.
- Learned that passwords are stored as cryptographic hashes.
- Understood the authentication process where hashes are compared during login.
- Analyzed how the “Forgot Password” feature works using reset tokens instead of password recovery.

---

### 2. Hashing vs Encryption
- Learned that hashing is a one-way process and cannot be reversed.
- Understood that encryption is a two-way process using secret keys.
- Analyzed why encryption is not suitable for password storage.
- Concluded that hashing provides better protection against data breaches.

---

### 3. Hash Types and Strength Analysis
Studied common hashing algorithms including:
- MD5 (weak and deprecated)
- SHA-1 (cryptographically broken)
- SHA-256 (strong but fast)
- bcrypt (recommended for password storage)

Compared their speed, security level, resistance to attacks, and real-world usage.

---

### 4. Practical Hash Generation
- Created a list of 5–10 test passwords.
- Generated MD5 and SHA-1 hashes for each password.
- Observed that even small changes in passwords produced completely different hash values.
- Identified hash formats based on character length.

---

### 5. Practical Hash Cracking Using Hashcat
- Used Kali Linux and Hashcat for password cracking demonstration.
- Created hash files for MD5 and SHA-1.
- Used the rockyou.txt wordlist for dictionary-based attacks.
- Successfully cracked multiple weak password hashes.
- Observed that common passwords were cracked instantly due to their presence in wordlists.

Hashcat modes used:
- MD5 → `-m 0`
- SHA-1 → `-m 100`

---

### 6. Attack Types Studied

#### Dictionary Attack
- Uses predefined wordlists containing commonly used passwords.
- Extremely fast and effective against weak passwords.
- Most successful real-world password attack.

#### Brute Force Attack
- Tries all possible character combinations.
- Slower but guaranteed to succeed for short passwords.
- Becomes impractical for long and complex passwords.

---

### 7. Analysis of Why Weak Passwords Fail
- Short password length
- Common words and patterns
- Lack of symbols and complexity
- Predictable formats (e.g., admin123, welcome@123)
- Presence in leaked password databases

---

### 8. Multi-Factor Authentication (MFA)
- Studied MFA as an additional security layer.
- Understood how MFA protects accounts even if passwords are compromised.
- Learned that MFA significantly reduces account takeover risks.

---

### 9. Security Recommendations
- Use long and complex passwords (12–16+ characters).
- Avoid common words and predictable patterns.
- Use password managers for unique credentials.
- Store passwords using bcrypt or other adaptive hashing algorithms.
- Implement salting to prevent rainbow table attacks.
- Enable Multi-Factor Authentication.
- Apply rate limiting and account lockout mechanisms.
- Educate users about password hygiene and phishing risks.

---

## Tools Used
- Kali Linux
- Hashcat
- Linux hashing utilities (`md5sum`, `sha1sum`)
- rockyou.txt wordlist

---

## Files Included
- Password hash files (MD5 and SHA-1)
- Screenshots of hash generation and cracking results
- Analysis documentation
- README.md

---

## Learning Outcome

Through this task, I gained a strong understanding of password security fundamentals, hashing mechanisms, common attack techniques, and defensive strategies used to protect authentication systems. This task provided hands-on exposure to how weak passwords can be compromised and why modern security practices such as strong hashing and MFA are critical in cyber security.

---

## Conclusion

This task demonstrated that passwords alone are not sufficient for securing accounts. Weak hashing algorithms and predictable passwords can be cracked easily using automated tools. Implementing strong password policies, secure hashing algorithms, salting, and multi-factor authentication is essential to protect systems from credential-based attacks.

---
