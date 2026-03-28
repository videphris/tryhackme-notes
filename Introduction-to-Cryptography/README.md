**Date:** 3/26/2026 
**Room URL / ID:**  https://tryhackme.com/room/cryptographyintro

**Goal / Objective:**  
--- 1–2 lines describing the main learning objective
Learn about symmetric, asymmetric

### Core Concept (In My Own Words)
--- Explain the main idea simply and clearly
Symmetric key encryption is used for efficient and secure communication utilizing the same key to decrypt and encrypt. Example programs are OpenSSL and GPG.

Asymmetric key encryption is best used to set up symmetric key encryption (as symmetric is more efficient) by having both a public and private key for encryption and decryption. For example, if a file is encrypted with the public key it can only be decrypted with the private key and vice versa. If it not possible to obtain the private key from knowing someone's public key. These two keys are mathematically linked. 
-Diffie-Hellman assymetric key exchange is what is used to allow exchange of a secret over a public channel.
-Incredibly difficult mathematical equations are used in assymetric encryption. It is easy to multiply two prime numbers but hard to factor them.

HMAC is verifying integrity by hashing with a key. This is much like a stamped and sealed letter proving integrity.

PKI (Public Key Insfrastructure) is how we prevent MITM attacks when using the Diffie-Hellman assymetric key exchange. We create certificate like with openSSL and get it signed with a trusted CA authority (like Digicert which is trusted by many browsers). 
SSL/TLS handshake occurs after the browser receives a signed certificate it trusts. When you get the untrusted website message that website is not validated by a certificate authority.
Signing means that after the SSL/TLS certificate is received, the Certificate Authority signs the hash of the certificate with their private key then appends it to the certificate. If the certificate authority is trusted, the third party will decrypt the hash using the CA's public key and compare it with the certificate.

After the TLS/SSL handshake this commences secret key with the diffie-hellman exchange then symmetric encryption for speed.

Hashing - a one way cryptographic function to store passwords securely. Commonly, a randomly generated salt is appended to the password pre-hash. The salt is public but makes it more resource intensive for attackers as they have to brute force each user.

SSL/TLS protects data in transit
Hashing protects data at rest. Hashing is secure when passwords are salted as rainbow tables deplete the security for hashing.

### Why It Matters
--- Why does this matter? What problem does it solve?

### How It Works
--- How do we do this? (short steps or explanation)

### Key Commands
--- Anything worth keeping

### Example / Use Case
--- Real-world or lab scenario

### What Confused Me / Slowed Me Down
--- Where I got stuck

### Key Takeaway
--- Single sentence I want to remember
