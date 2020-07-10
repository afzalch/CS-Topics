## Table of Contents
- [Cryptographic Tools](#cryptographic-tools)
- [Certificates](#certificates)


## Cryptographic Tools



**Symmetric Encryption** - same key is used to encrypt and decrypt
- Universal technique for providing confidentiality for transmitted or stored data
- Two requirements for secure use
  - Strong encryption algorithm
  - Sender and receiver must have received copies of key in a secure fashion and must keep the key secure

The problem with symmetric encryption is how are the keys shared


Asymmetric Encryption - one key is used to encrypt and another key is used to decrypt
Server distributes public key publicly while private key is kept hidden and used to decrypt any messages sent that have been encrypted using the public keys
 
Cons is that it is slower than symmetric encryption because keys can be quite a fair bit larger than the keys used in symmetric encryption

HTTPS:
Need to trust that public key cryptography and signature works
1) Any message encrypted with public key can only be decrypted with their private key
2) Anyone with access to __ public key can verify that a message (signature) could only have been created by someone with access to ___'s private key 


## Certificates
- Electronic credentials used to assert the identities of individuals, computers and other entities on a network
- Similar to ID cards (driver licenses, passports, etc)
- Contain public key and identity of the owner
 
- One of the more common uses of certificates is in SSL 

### Certificate Issuer
- Issues by a certificate authority (CA) that validates the identity of the certificate holder
- Great way to prevent a man-in-the-middle attack as the CA wouldn't validate the man-in-the-middle


**Certificate Signing Request (CSR)**
Can be done through the use of programs such as openSSL that create a private key and a CSR from scratch 