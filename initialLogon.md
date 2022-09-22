Building a Zero Trust Architecture that works for you!

Zero Trust Architecture Initial Log on Goals

1. Never Trust, Always Validate
2. Every connection is a potential threat
3. Defend against attacks and scams that could infiltrate the system

Zero Trust Architecture Initial Log on
 
Asset Discovery (What are the important assets on this network?)
    - Use automated tools to discover assets on the network or query procurement records
    - Know what data is being stored, the location, and its sensitivity
    - Access policies that authorize requests will be based on sensitivity of data
    - Conduct risk assessment to see if Zero Trust Implementation will protect against all risks or at least mitigate the risks

Provision users
    - Single User directory
    - Specify users who can access specific areas and what security measures they will use to access them (Level of Multi-factor Authentications(MFA)Low-High)
    - User Credentials are Username, Password(FIDO2), and use MFA YubiKeys
    - Assign each user a role based on work they will be performing
    - User accounts will configured to be least privilege
    - Single sign on for users to access all services within the Zero Trust Architecture
    - Another option is to group users into a "group"(sudo addgroup) together and grant specific privileged access to the group
 
Device Authentication (What are the devices on this network? Administrator provided? or BYOD?)
    - Use hardware co-processor, such as a Trusted Platform Module (TPM), which will give high confidence in the device's identity
    - Key attestation should be used where possible to prove the identity is protected in a secure hardware co-processor
    - Entity requesting a certificate will prove to certificate authority that the RSA key in the certificate request is protected by TPM a certificate authority trust
    - Each Device should be uniquely identifiable in a single device directory
    - On an unmanaged device, using a software-based key store provides the least amount of confidence in the device's identity
    - Devices in a BYOD model should still have an identity linked to them, but the confidence in that device's identity will be low

Certificate Distribution
    - Transport Layer Security (TLS) is responsible for issuing TLS certificates
    - The TLS is allowing the application to have a strong cryptographic identity (Service Identity)
    - Encryption of all traffic
    - Automatic Generation of a Public/Private Key pair in memory
    - For example see diagram below
    - Generate Key pair -> Client -> Generate a certificate signing request -> Server -> Sign Certificate
    - Server Says "I am a public key and a server! Please sign me certificate authority!"
    - Certificate Authority says "Are you a Web server and should you be allowed to have this certificate? If yes then I will sign it"
    - Short lived keys automatic generation and rotation

Service Discovery
    - Service Configuration
    - Service Segmentation

The superuser (root) has complete access to the operating system and its configuration; it is intended for administrative use only. Unprivileged users can use the su and sudo programs for controlled privilege elevation.
