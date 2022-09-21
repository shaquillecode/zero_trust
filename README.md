Introduction to Zero Trust Architecture

We must eliminate the notion of a trusted network (intranet) and an untrusted network (external networks). In Zero Trust, all network traffic is untrusted.

Traditional Perimeter Security Model are problematic

Traditional Perimeters Security Model are very difficult to manage in a world of microservices. Cloud computing service communication requirements are constantly changing. Traditional tools for internal access need to be adapted (ie Digital Identity)

Initial Log on Goals

1. Never Trust, Always Validate
2. Every connection is a potential threat
3. Administrators will grant everyone least privilege access

Initial Log on  Implementation

1. Asset Discovery ( What’s  important on this system? Rank security level of Asset)
2. Authenticate and Authorize Everywhere
3. Specify users who can access specific areas and what security measures they will use to access them. (Level of Multi-factor Authentications(MFA))
4. User Credentials are Username, Password(FIDO2), and MFA YubiKeys

Demo
(See more for TPM (Trusted Platform Module) computer chip (microcontroller) RSA,BIOS,Two Factor Authentication, User/Device/Service health check.)

Managing users is done for the purpose of security by limiting access in certain specific ways. The superuser (root) has complete access to the operating system and its configuration; it is intended for administrative use only. Unprivileged users can use the su and sudo programs for controlled privilege elevation.

Any individual may have more than one account as long as they use a different name for each account they create. Further, there are some reserved names which may not be used such as "root".

Users may be grouped together into a "group", and users may be added to an existing group to utilize the privileged access it grants.

Username/Password/MFA verifies

Confirm user is active in Lightweight Directory Access Protocol (LDAP)
Populate, department, roles, TLS cert verifies

Lookup in device database for lost/stolen, confirm host firewall, config, patch, vulndb
Ip address is local/ remote/ banned, Looks for patterns of misuse

Filter roles, groups, deny based on policy
