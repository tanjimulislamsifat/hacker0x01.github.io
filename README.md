# Subdomain Takeover POC

A proof-of-concept (POC) demonstration page for subdomain takeover vulnerabilities.

## Overview

This HTML page serves as a visual proof-of-concept to demonstrate successful subdomain takeover attacks. It's designed to clearly indicate when a subdomain has been compromised due to misconfigured DNS settings.

## Features

- **Clear Visual Indicators**: Red warning headers and yellow warning text to immediately show the takeover
- **Professional Styling**: Dark theme with contrasting colors for high visibility
- **Responsive Design**: Mobile-friendly viewport configuration
- **Attribution**: Includes researcher identification

## File Structure

```
subdomain-takeover-poc/
├── index.html          # Main POC page
└── README.md          # This documentation
```

## Usage

1. **For Security Researchers**: 
   - Deploy this page to demonstrate subdomain takeover vulnerabilities
   - Use as evidence in responsible disclosure reports
   - Include in penetration testing documentation

2. **For Domain Owners**:
   - If you see this page on your subdomain, immediately secure your DNS settings
   - Review all CNAME records and remove dangling references
   - Implement proper subdomain monitoring

## Security Implications

Subdomain takeover occurs when:
- A subdomain points to an external service (via CNAME)
- The external service account/resource is deleted or becomes unclaimed
- An attacker claims the external resource
- The attacker can now serve content on your subdomain

## Mitigation Steps

1. **Audit DNS Records**: Regularly review all DNS entries
2. **Remove Unused Subdomains**: Delete CNAME records for discontinued services
3. **Monitor Subdomains**: Implement automated monitoring for unexpected changes
4. **Use DNS Security**: Consider DNS security solutions and monitoring tools

## Technical Details

- **Language**: HTML5 with embedded CSS
- **Browser Support**: All modern browsers
- **Dependencies**: None (self-contained)
- **Size**: Lightweight (~1KB)

## Responsible Disclosure

This tool is intended for:
- ✅ Authorized security testing
- ✅ Responsible vulnerability disclosure
- ✅ Educational purposes
- ✅ Bug bounty programs

**Not for:**
- ❌ Unauthorized testing
- ❌ Malicious activities
- ❌ Defacement or harm

## License

This project is provided for educational and security research purposes. Use responsibly and in accordance with applicable laws and regulations.

## Author

**Tanjimul Islam Sifat**

For questions about this POC or responsible disclosure, please contact through appropriate security channels.

