# Encryption Commands Cheat Sheet

## Symmetric Encryption
- AES: `openssl enc -aes-256-cbc -in plaintext.txt -out encrypted.txt`

## Asymmetric Encryption
- RSA encrypt: `openssl rsautl -encrypt -inkey public.pem -pubin -in message.txt -out message.enc`
- RSA decrypt: `openssl rsautl -decrypt -inkey private.pem -in message.enc -out message.txt`

## Hashing
- SHA-256: `sha256sum file.txt`
- MD5: `md5sum file.txt`

## Digital Signatures
- Sign: `openssl dgst -sha256 -sign private.pem -out signature.bin file.txt`
- Verify: `openssl dgst -sha256 -verify public.pem -signature signature.bin file.txt`
