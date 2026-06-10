# CONCLUSION

This project demonstrated a complete Active Directory attack lifecycle within a controlled lab environment. Starting from initial enumeration, a password spraying attack was used to gain access to a low-privileged user account.

Further exploitation through Kerberoasting allowed extraction of a service account hash, which was used to obtain higher privileges within the domain. Ultimately, administrative access was achieved, enabling the extraction of the Active Directory database (NTDS.dit), resulting in full domain compromise.

The assessment highlights how weak password policies, improper service account configurations, and lack of monitoring can lead to severe security breaches in enterprise environments. It emphasizes the importance of implementing strong security controls, least privilege principles, and continuous monitoring to protect Active Directory infrastructures.
