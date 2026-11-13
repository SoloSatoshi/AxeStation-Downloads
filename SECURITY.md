# Security

Report suspected vulnerabilities privately through the contact options at
[solosatoshi.com](https://www.solosatoshi.com/). Do not post passwords, access
tokens, personal network details or unredacted logs in public issues.

Official application update metadata is signed. AxeStation verifies the signature,
platform-specific download location, file size and SHA-256 checksum before
installation. A previous application copy is retained until the updated app
acknowledges startup. Update signing is separate from operating-system code
signing; Windows builds are unsigned and Mac builds are ad-hoc signed.

Miner administration APIs are intended for trusted local networks. Do not expose
miners or AxeStation helper services directly to the internet.
