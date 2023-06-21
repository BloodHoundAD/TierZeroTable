# TierZeroTable
Table of AD and Azure assets and whether they belong to Tier Zero.

Blog post: [What is Tier Zero - Part 1](https://posts.specterops.io/what-is-tier-zero-part-1-e0da9b7cdfca)

Webinar: [Defining the Undefined: What is Tier Zero](https://specterops.zoom.us/webinar/register/WN_hOwvqBQ3Q7-9dGS-urDj9w)

**DISCLAIMER: The table does not include all Tier Zero assets yet.** We will add assets to the table throughout the webinar series. So if you think we are missing something, then you are completely right. But feel free to make a pull request or open an issue with the asset you think we should add. All contributions are appreciated. Also if you disagree on something in the table :)

# Table columns

### Name
Common name of the asset.

### Type
Type of the asset.

Values:
- AD group
- DC group

### IdP
Identity Provider of the asset.

Values:
- Active Directory

### Identification
How the asset can be identified. E.g., SID of AD object.

### Description
Description of the asset, i.e., its purpose of existence. This will be copied from Microsoft documentation if available.

### Known Tier Zero compromise abuse
Whether a publicly known abuse exists that allows compromise of Tier Zero assets using this asset. The abuse has to be described publicly in detail to an extent that others can replicate the abuse. POC||GTFO :)

If a publicly known abuse exists it will be described in the _Reasoning_ column and links will be provided in the _External links_ column.

Values:
- YES - A publicly known abuse exists and works in environments with common configurations.
- DEPENDS - A publicly known abuse exists and works in some environments depending on configurations etc.
- NO - No known abuse exists.

### Is Tier Zero
If the asset should be considered Tier Zero based on our [Definition of Tier Zero](https://github.com/JonasBK/TierZeroTable/tree/main#definition-of-tier-zero).

### Reasoning
The explanation of why the asset is/isn't Tier Zero, including an abuse summary and if the asset is a security dependency for Tier Zero.

### Microsoft: Privileged access security roles
Whether the asset is included in Microsoft's [Privileged access security roles](https://learn.microsoft.com/en-us/security/privileged-access-workstations/privileged-access-security-levels) list.

Values:
- YES
- NO

### AdminSDHolder protected
Whether the asset is part of the default [Protected Accounts and Groups in Active Directory](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/plan/security-best-practices/appendix-c--protected-accounts-and-groups-in-active-directory), which are protected with the AdminSDHolder security descriptor.

Values:
- YES
- NO

### External links
Links to documentation for the asset, abuse information, etc.
