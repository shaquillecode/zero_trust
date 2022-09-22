Building a Zero Trust Network that works for you!

Zero Trust Initial Log on Goals

1. Never Trust, Always Validate
2. Every connection is a potential threat
3. Administrators will grant everyone least privilege access

Zero Trust Initial Log on Implementation
 
1.Asset Discovery (What are the important assets on this network?)
  -Use automated tools to discover assets on the network or querying procurement records
  -Know what data is being stored, the location, and its sensitivity
  -Access policies that authorize requests will be based on sensitivity of data
  -Conduct risk assessment to protect against all risks or at least mitigate the risks

2. Find your users, devices, and the services and data they are accessing

3. Provision Strong user Authentication
    -Use single User directory for effiency
    -Specify users who can access specific areas and what security measures they will use to access them. (Level of Multi-factor Authentications(MFA))
    -User Credentials are Username & Password(FIDO2), and use MFA YubiKeys
    -Assign each user a role based on work they will be performing
    -User accounts will configured to be least privilege
    -Single sign on for users to access all services within the Zero Trust Architecture
    -Users may be grouped together into a "group", and users may be added to an existing group to utilize the privileged access it grants

4. Device Authentication (What are the devices on this network? Adminstrator provided? or BYOD?)
     -Device health check
       - Each Device should be uniquely identifiable in a single device directory. This enables efficient asset management
       -Using a secure hardware co-processor, such as a Trusted Platform Module (TPM), will give you high confidence in the device's identity. Key attestation should be used where possible to prove the identity is protected in a secure hardware co-processor.
       -On an unmanaged device, using a software-based key store provides the least amount of confidence in the device's identity, relative to the above.
       -Devices in a BYOD model should still have an identity linked to them for monitoring purposes, but the confidence in that device's identity would likely be lower.
5. Certificate Distribution
     -Transport Layer Security (TLS) Responsible for issuing TLS certificates
     -The TLS is allowing the application to have a strong crytographic identity (Service Identity)
     -Encryption of all traffic
     -Automatic Generation of a Public/Private Key pair in memory
     -Generate Key pair->Client->Generate a certificate signing request=>Server->Sign Certificate
     -"I am a public key and a server! Please sign me certificate authority!"
     -"Are you a Web server should you be allowed to have this certificate? If yes then I will sign it."
     -Short lived keys automatic generation and rotation
6. Service Discovery
     -Servce Configuration
     -Service Segmentation
Demo
(See more for RSA,BIOS,etc)

Managing users is done for the purpose of security by limiting access in certain specific ways. The superuser (root) has complete access to the operating system and its configuration; it is intended for administrative use only. Unprivileged users can use the su and sudo programs for controlled privilege elevation.
