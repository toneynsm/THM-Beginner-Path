## Windows Essentials

## Resources
- Configure rules with group policy: https://learn.microsoft.com/en-us/windows/security/operating-system-security/network-security/windows-firewall/configure
- Intro to Alternate Data Streams (ADS): https://www.malwarebytes.com/blog/101/2015/07/introduction-to-alternate-data-streams
- System Configuration Troubleshooting guide: https://learn.microsoft.com/en-us/troubleshoot/windows-client/performance/system-configuration-utility-troubleshoot-configuration-errors
- Overview of BitLocker: https://learn.microsoft.com/en-us/windows/security/operating-system-security/data-protection/bitlocker/

## Active Directory Notes
- Difference between organizational units (OUs) and security groups: organizational units are like blanket rules (applied policies) to any user WITHIN that OU, whereas security groups are like EXCEPTIONS, or more NICHE rules, if you will. Security groups relate to a SPECIFIC permission. So it's like:\
A user will typically be apart of an OU with specific policies applied (i.e. they're apart of a certain dept., can only access certain resources, etc.), BUT, they need access to a specific folder or application that's OUTSIDE the perview of their OU, so they're included in a group that SPECIFIES access to that one particular resource
\
\
OU and Group Policy Pipeline is basically:
1. Create OUs (Sales, Marketing, IT, etc.)
2. Create Group Policy Objects (GPOs), which are the policies/configurations themeselves
3. **APPLY** the GPO to a specific OU (i.e. prohibit access to this resource to ALL users in this OU)
