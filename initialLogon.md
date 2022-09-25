Introduction to Zero Trust Architecture

The superuser (root) has complete access to the system and its
configuration. In a Zero Trust Architecture it is intended for admin use
only!

Provision users
- Single User directory
- Set Level of Multi-factor Authentications(MFA) and rank MFA Low - High
- Use One Time passcode and Security Token to authenticate
- Use Security Token YubiKey based on Two-factor authentication
- Use passwordless authentication using a device with FIDO2
- User accounts will configured to be least privilege
- Generate a public/private rsa key pair for single sign on within ZTA
# ssh-keygen -b 4096

Device Authentication (What are the devices on this network?)
- Use hardware co-processor, such as a Trusted Platform Module (TPM)
- Use Key attestation to prove the identity is protected in a TPM
- Entity requesting a certificate will have to prove to certificate
authority that the RSA key in the certificate request is protected by TPM a certificate authority can trust
- Single device directory and each Device will be uniquely identifiable
- Devices in a BYOD model the device's identity level is low

Certificate Distribution
- Transport Layer Security (TLS) is responsible for certificates
- The TLS is allowing the application to have a strong cryptographic
identity (Service Identity)
- Encryption of all traffic
- For example see below
- Generate Key pair -> Client -> Generate a certificate signing
request -> Server -> Sign Certificate
- Server Says "I am a public key and a server! Please sign me
certificate authority!"
- Certificate Authority says "Are you a Web server and should you be
allowed to have this certificate? If yes then I will sign it"