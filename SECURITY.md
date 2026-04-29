# Security Policy

## Reporting Security Vulnerabilities

**Please do not report security vulnerabilities in public GitHub Issues.**

If you discover a security issue in Furya, please contact us at: [security@anigx.dev](mailto:security@anigx.dev)

## Supported Versions

| Version | Supported          |
| ------- | ------------------|
| v1.5.x  | :white_check_mark: |
| v1.4.x  | :white_check_mark: |
| < v1.4  | :x:                |

## Security Best Practices

### Protect Your API Key
- Never share your API key with anyone
- Do not post your API key in public GitHub Issues
- Use a device lock screen (PIN, password, biometric)
- Remove your account from Furya before selling or giving away your device

### Official Downloads Only
**Only download Furya from:**
- The official [GitHub Releases](https://github.com/Anigx/Furya-Public/releases) page
- The in-app updater

**Never download Furya from:**
- Third-party APK hosting sites
- Unknown links in comments or messages

### Verify Your Download
Each release includes a SHA-256 checksum file (`.sha256`). To verify:
1. Download both the APK and the `.sha256` file
2. Run: `sha256sum -c Furya-vX.X.X-bXX.apk.sha256`
3. Verify the output shows "OK"

## Responsible Disclosure

We appreciate responsible disclosure of security issues. Please contact us directly before publishing any vulnerability details.