# 04 · Introduction to Cryptography

Cryptography supports **confidentiality**, **integrity**, **authentication**, and (via signatures) **non-repudiation**.

| Building block | Key idea | Examples |
|----------------|----------|----------|
| Symmetric encryption | One shared secret key; fast, but key sharing is hard | AES (modern), 3DES (legacy), DES (obsolete) |
| Asymmetric encryption | Public/private key pair; slower; key exchange and signatures | RSA, ECC |
| Hashing | One-way fixed-length digest; integrity, file identification | SHA-256 |
| HMAC | Hash + shared secret; integrity and authenticity | HMAC-SHA256 |
| Digital signature | Sign with private key, verify with public key | RSA/ECDSA signatures |
| Certificates / PKI | CAs bind a public key to an identity; basis of HTTPS | X.509 |

**Passwords:** store with a salted, slow KDF (Argon2, bcrypt, scrypt, PBKDF2), not a fast hash alone.
**Hybrid cryptography:** asymmetric methods authenticate and establish keys, then symmetric encryption protects the data (this is how **TLS** works).
**Not the same:** a signature is not encryption; encryption alone does not guarantee integrity.

## 🔵 Blue Team checkpoint
- Encryption → confidentiality · Hashing → detects change · Signatures → origin + integrity
- Check certificate validity and identity in TLS issues
- A matching hash doesn't prove a file is safe
- Exposed private keys, weak algorithms, and poor key handling are concerns; encrypted traffic itself is normal, so assess context and endpoints
