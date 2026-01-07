# Network Automation Projects

Practical Python automation projects focused on **network reliability**, **observability**, and **configuration management**.

This organization hosts a curated set of tools built to demonstrate real-world skills used in **Network Reliability Engineering (NRE)**, **SRE**, and **DevOps** roles.

---

## Focus Areas

- Automating configuration management and device interaction  
- Building observability and monitoring workflows  
- Collecting, storing, and querying telemetry data  
- Applying best practices:
  - structured logging  
  - error handling  
  - CLI interfaces  
  - maintainable, readable code  

---

## Projects

### Config File Automator
Python CLI tool for safe backup and recursive modification of YAML and JSON configuration files.

**Key features**
- Timestamped backups before changes  
- Recursive placeholder replacement in nested structures  
- Comprehensive logging and robust error handling  

**Use case**  
Automating configuration updates across network services or devices.

---

### Network Telemetry Manager
Python tool for storing, querying, and analyzing mock network telemetry data using SQLite.

**Key features**
- Stores metrics (latency, packet loss, etc.) per device  
- Aggregation queries (e.g. average latency)    
- JSON export for dashboards or APIs  

**Use case**  
Simulates observability pipelines similar to Prometheus, Grafana, or SolarWinds-style workflows.

---

### Netmiko Network Device Tool *(in progress)*
Netmiko-based automation for interacting with Cisco IOS-XE devices using SSH.

**Planned features**
- Execute `show` commands against real devices (DevNet sandbox)  
- Capture structured output  
- Save results as TXT / JSON  
- Full session logging  

**Use case**  
Hands-on practice with live network device automation.

### Ansible Network Automation

Ansible playbooks for automating common Cisco IOS workflows in sandbox environments.  falls back to mock data when sandbox is not available.

Key features:
- Configuration backups
- Device fact gathering
- Basic validation checks
- Idempotent, repeatable runs

Use case:
Practicing declarative network automation and validating configurations safely using Ansible.

### API & Infrastructure Tooling (Hands-on Labs)

In addition to the repositories here, I’ve completed structured hands-on labs focused on building and testing RESTful APIs using Python and FastAPI.

These labs covered:
- CRUD API design
- OAuth-based authentication flows
- MongoDB-backed data models
- Request validation with Pydantic
- Introductory scalability and API testing concepts

This work complements the automation projects by strengthening API design and service integration skills.

---

## Motivation

These tools were built as targeted preparation for roles involving:

- Automation of network provisioning and configuration  
- Interfacing with network devices and APIs  
- Designing internal observability systems  
- Reducing operational toil through reliable scripting  

The projects reflect common expectations such as Python proficiency, familiarity with Netmiko/NAPALM, telemetry data handling, and SRE-oriented thinking.

---

## Maintenance

Maintained by **Rebecca Clarke**  
Software Engineer — Network Automation & Reliability  

Primary portfolio work for this domain lives within this organization.

LinkedIn: https://www.linkedin.com/in/rebecca-clarke-0a8b082b/

---

More tools planned, including:
- Terraform wrappers  
- Ansible integrations  
- Monitoring and visualization dashboards  

Feel free to explore, fork, or star the repositories. Feedback via issues is welcome.
