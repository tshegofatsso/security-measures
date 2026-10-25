# Global Security Advisory Monitoring and Measures

This repository implements automated security practices based on the GitHub Global Security Advisory Database.

## Recent Critical and High Severity Advisories (as of Oct 2026)

- **Wasmtime (Rust)**: GHSA-897f-g5gm-fmxm / CVE-2026-115889 - Critical miscompilation leading to sandbox escape. Upgrade to v36.0.19+ or v43+.
- **Pillow (Python/pip)**: Heap buffer overflow in FlashPix JPEG decoding. Critical code execution. Update Pillow.
- **virtualenv (pip)**: Multiple high severity prompt injection issues in activation scripts. Upgrade to 21.14.9+.
- **Vite (npm)**: Several high severity arbitrary file read and path bypass issues in older versions (<8.x). Upgrade recommended.
- **Bun (npm)**: Compromised root certificates. Upgrade to 1.4.4+.

## Implemented Measures

1. Dependabot configurations pushed to key private repositories (GreenMan-PoS, mgsn-site) for weekly dependency updates.
2. SECURITY.md policies added.
3. Branch protection attempted (requires GitHub Pro for private repos).
4. Ongoing monitoring of global advisories for npm, pip, and other ecosystems used.

## Next Steps

- Enable Dependabot alerts in repository settings if not automatic.
- Review and upgrade vulnerable packages (e.g., vite).
- Consider making critical repos public or upgrading plan for advanced rulesets.
- Regularly check https://github.com/advisories

Stay secure by keeping dependencies updated and reviewing advisories.
