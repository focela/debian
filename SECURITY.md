# Security Policy

## Overview

This document outlines our security policies, supported versions, vulnerability reporting procedures,
and recommended security best practices for users of this Docker image.

## Supported Versions

We maintain a focused support policy to ensure optimal security:

| Version              | Support Status | Security Updates |
|----------------------|----------------|------------------|
| Latest (main branch) | ✅ Supported   | Regular updates  |
| Older tags           | ❌ Unsupported | No updates       |

> **Note:** Always use the latest version to ensure you have all security patches and updates.

## Vulnerability Reporting

If you discover a security vulnerability, please follow these steps:

1. **Do not disclose the vulnerability publicly** (no GitHub issues, forums, etc.)
2. Send a detailed report to: **security@focela.com**
3. Include relevant information such as:
    - Description of the vulnerability
    - Steps to reproduce
    - Potential impact
    - Suggested mitigation (if any)

### Response Timeline

Our security team follows this process:

- **Acknowledgment:** We will acknowledge your report within 72 hours
- **Investigation:** We will investigate the reported vulnerability promptly
- **Resolution:** We will work to address valid vulnerabilities as quickly as possible
- **Disclosure:** We will coordinate responsible disclosure if necessary

## Security Best Practices

When using this Docker image, we recommend the following security measures:

1. **Keep Updated**
    - Always pull the latest tag to ensure up-to-date dependencies
    - Subscribe to release notifications if available

2. **Privilege Management**
    - Use minimal privileges when deploying containers based on this image
    - Configure appropriate user permissions within containers

3. **Configuration Security**
    - Disable unused features via environment variables when possible
    - Avoid exposing unnecessary ports
    - Use secrets management for sensitive configuration values

4. **Monitoring**
    - Implement monitoring for containers based on this image
    - Regularly review logs for suspicious activities
