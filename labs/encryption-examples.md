# Lab: Encryption Examples

- Symmetric Encryption Example:
  ```bash
  openssl enc -aes-256-cbc -in plaintext.txt -out encrypted.txt
  ```
Asymmetric Encryption Example:

```bash
openssl rsautl -encrypt -inkey public.pem -pubin -in message.txt -out message.enc
```

Hashing Example:

```bash
sha256sum file.txt
```
