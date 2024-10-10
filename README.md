### Generate Keypair
#### Summary
A keypair is a matching pair of public key and secret key.
The public key is used as an “address” that points to an account on the Solana network. A public key can be shared with anyone.
The secret key is used to verify authority over the account. As the name suggests, you should always keep secret keys secret.
@solana/web3.js provides helper functions for creating a brand new keypair, or for constructing a keypair using an existing secret key.
#### Lesson
In this lesson, we will explore the basics of cryptography and how it's applied within the Solana ecosystem.

#### Symmetric and Asymmetric Cryptography
'Cryptography' the study of hiding information. There are two main types of cryptography you'll encounter day to day:

#### Symmetric Cryptography 
is where the same key is used to encrypt and decrypt. It's hundreds of years old and has been used by everyone from the ancient Egyptians to Queen Elizabeth I.

There's a variety of symmetric cryptography algorithms, but the most common you'll see today are AES and Chacha20.

#### Asymmetric Cryptography
- Asymmetric cryptography - also called 'public key cryptography' was developed in the 1970s. In asymmetric cryptography, participants have pairs of keys (or keypairs). Each keypair consists of a secret key and a public key. Asymmetric encryption works differently from symmetric encryption, and can do different things:
- Encryption: if it's encrypted with a public key, only the secret key from the same keypair can be used to read it
- Signatures: if it's encrypted with a secret key, the public key from the same keypair can be used to prove the secret key holder signed it.
- You can even use asymmetric cryptography to work out a good key for symmetric cryptography! This is called key exchange, where you use your public keys and the recipient's public key to come up with a 'session' key.
- There's a variety of asymmetric cryptography algorithms, but the most common you'll see today are variants of ECC or RSA.
