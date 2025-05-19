# Changelog

All notable changes to this project will be documented in this file.  
This project adheres to [Semantic Versioning](https://semver.org/).

## [7.10.31] - 2025-05-19

### Added

#### Core Components
- **S6 Overlay**: 3.2.0.3
- **Zabbix Agent**: 7.2.6
- **Fluent-Bit**: 3.1.10
- **YQ**: 4.44.1
- **GoLang**: 1.24.2
- **OpenDoas**: 6.8.2

#### Key Features
- Multi-architecture support (`amd64`, `arm64`, `arm/v7`)
- Comprehensive process management using **S6 Overlay**
- Monitoring via **Zabbix Agent** (classic/C & modern/Go implementations)
- Log management and shipping with **Fluent-Bit**
- Security hardening using **Fail2ban** and firewall rules
- Messaging support via **MSMTP**
- Cron-based scheduling (BusyBox)
- Dynamic user/group ID management

#### Main Functions
- Container initialization and lifecycle management
- Service control (start/stop/status)
- Database connectivity check
- Log rotation and compression
- Template file management
- Git operations
- Process watchdog & runaway protection
- Custom script hooks and execution

#### Environment Variables
- **Container config**: `CONTAINER_NAME`, `TIMEZONE`, `DEBUG_MODE`
- **Monitoring**: `CONTAINER_ENABLE_MONITORING`, `ZABBIX_AGENT_TYPE`
- **Logging**: `CONTAINER_ENABLE_LOGSHIPPING`, `CONTAINER_ENABLE_LOGROTATE`
- **Security**: `CONTAINER_ENABLE_FIREWALL`, `CONTAINER_ENABLE_FAIL2BAN`
- **Messaging**: `CONTAINER_ENABLE_MESSAGING`, `SMTP_HOST`, `SMTP_PORT`
- **Scheduling**: `CONTAINER_ENABLE_SCHEDULING`
- **Process protection**: `CONTAINER_PROCESS_RUNAWAY_PROTECTOR`
- **Custom behavior**: `CONTAINER_POST_INIT_COMMAND`, `CONTAINER_POST_INIT_SCRIPT`
