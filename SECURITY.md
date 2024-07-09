# Security Policy

```[!NOTE]
This document is a work in progress as we work to find a safe and secure route to vulnerability reporting.
```

If you find a potential or confirmed vulnerability in the distributable code of this project, please DO NOT FILE AN ISSUE. Instead, please email the Director of Web Strategy directly with all technical details on how exactly to exploit the vulnerability and how that exploitation may be abused.

When possible, as a vulnerability reporter, we recommend you avoid:

- Disclosing the vulnerability publicly without giving maintainers a chance to remediate.
- Bypassing the maintainers.
- Disclosing the vulnerability before a fixed version of the code is available.
- Expecting to be compensated for reporting an issue, where no public bounty program exists.

## Standard security remediation protocol

1. When a vulnerability is reported we must acknowledge receipt of the vulnerability report as quickly as possible, even if no immediate resources are available for investigation.
2. We will involve the vulnerability reporter when we verify the impact and veracity of the report.
3. A [draft GitHub Security Advisory](https://docs.github.com/en/code-security/repository-security-advisories/creating-a-repository-security-advisory) will be created for maintainers and vulnerability reporter to discuss and develop a fix on a private fork, taking any concerns and advice provided by the vulnerability reporter into careful consideration, and potentially seeking consultation or advice from security specialists if the patch for the vulnerability is beyond our team's experience or bandwidth.
4. A hotfix will be published to patch the vulnerability as soon as one has been developed, tested, and verified. The patch notes must indicate the update fixes a security vulnerability and credit the vulnerability reporter for the discovery.
5. After the hotfix has been live for an acceptable period of time, the details of the security vulnerability must be disclosed by [publishing the GitHub Security Advisory](https://docs.github.com/en/code-security/repository-security-advisories/publishing-a-repository-security-advisory).

### Security advisory content

A published security advisory must include the following points:

- A high level summary of the vulnerability, including the impact.
- A clear list of vulnerable versions.
- A clear list of patch versions.
- Any caveats on when the software is vulnerable (for example, if only certain configurations are affected)
- Any workarounds or mitigation that can be implemented as a temporary fix.
- Credit for the researcher who identified the vulnerability.

Optionally, a security advisory may include:

- Technical details of the vulnerability.
- A CVE for the vulnerability.
- IDS/IPS signatures or other indicators of compromise.

If a fix will not be available in the near future, a security advisory may be made public with minimal info, a timeline on when a fix for the vulnerability may be made and/or mitigation that can be implemented as a temporary fix.
