---
name: Bug Report or Feature Request
about: Create a new issue to report a bug or request a feature
title: "[Bug] <your title here>" or "[Feature] <your title here>"
labels: []
assignees: []

---

<!-- 
INSTRUCTIONS: 
This template helps maintainers quickly understand and address your issue.
Please fill in as much information as possible, deleting sections that don't apply.
-->

## Issue Type
<!-- Mark with an 'x' the type of issue this is [x] -->
- [ ] Bug Report
- [ ] Feature Request
- [ ] Documentation Issue
- [ ] Question/Support

## Description
<!-- Provide a clear and detailed explanation of the issue or feature request -->
A clear and concise description of what the issue or feature is.

<!-- For feature requests, explain the use case and benefits -->
<!-- For bugs, explain what's happening versus what you expected -->

## Steps to Reproduce (for bugs)
<!-- Detailed steps that would allow a maintainer to reproduce the issue -->
1. Pull image with `docker pull focela/debian:tag`
2. Run container with `docker run -e VARIABLE=value ...`
3. Run command `...` inside container
4. Observe error `...`

## Expected Behavior
<!-- What should have happened or what you'd like to see implemented -->
What you expected to happen.

## Actual Behavior (for bugs)
<!-- What actually happened - include any error messages, logs, or screenshots if available -->

## Environment Information
<!-- The more details you can provide, the better -->
- **Image version**: <!-- e.g. 7.10.31 -->
- **Container platform**: <!-- e.g. Docker, Podman, Kubernetes -->
- **Architecture**: <!-- e.g. amd64, arm64, armv7 -->
- **Host OS**: <!-- e.g. Ubuntu 22.04, CentOS 9, macOS 13.4 -->
- **Docker/container runtime version**: <!-- e.g. Docker 24.0.5 -->

## Configuration
<!-- Share relevant configuration details - remove sensitive information -->
```yaml
# Add your docker-compose.yml, environment variables, or other configuration here
