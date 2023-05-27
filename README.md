# htpk - HTTP Public Key Authentication

## All the security of passkeys using open-source protocols and credentials

Passkeys are great, but shouldn't require developers (and users!) to trust
proprietary keys stores like Google's Android Credential Manager or Apple's
iCloud Keychain

htpk is a secure, end-to-end open-source (e2eos), authentication system built
on transparent, proven, exsiting key fomats and protocols that are already
well-understood and familiar to developers:

1. public and private key pairs use the exact same file format as ssh keys

2. simple plain-text HTTP header-based protocol based on HTTP Basic Auth,
extended to negotiate a public key cryptographic challenge/response

3. server-side public key storage uses the same format as ssh `authorized_keys`
files. Clients use `.pem` encoded private keys
