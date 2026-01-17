# Network Automation Projects

Practical Python and Go automation projects focused on **network reliability**, **observability**, and **configuration management**.

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

### Go Prometheus Metrics Service
Lightweight Go service exposing custom Prometheus metrics to demonstrate application-level observability, metric instrumentation, and monitoring workflows commonly used in SRE and platform engineering environments.

This project implements a minimal HTTP service written in Go that publishes operational metrics in Prometheus format. It demonstrates how applications expose internal state for scraping, aggregation, and alerting in production monitoring systems.

**Key features**
Custom Prometheus metrics implemented using the Go Prometheus client
HTTP server exposing a /metrics endpoint
Example metrics like:
  Request counts
  Request duration
  Application health indicators
Designed to integrate with Prometheus scraping and Grafana dashboards

### Kubernetes Fundamentals Lab
Hands-on Kubernetes lab demonstrating core container orchestration concepts using Pods, Deployments, and Services. The lab progresses from fragile single-pod deployments to production-ready, self-healing, load-balanced applications.

**Key features**
Declarative Infrastructure using YAML manifests
Pod Lifecycle Management as the basic execution unit
ReplicaSets & Fault Tolerance through Deployments
Self-Healing via automatic pod replacement
Service Discovery with stable networking abstractions
Load Balancing across multiple replicas
Safe Teardown & Redeploy Workflows

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

### Netmiko Dashboard
First version simply imported netmiko class and showed mock data strings.  New version connects to Nokia practice servers using multiple concurrent connections with ThreadPoolExecutor, collects device facts and performs configuration backups in parallel, with data persisted in SQLite and exposed through a REST API.

**Planned features**
Concurrent SSH connections to multiple network devices using ThreadPoolExecutor

Device fact collection (hostname, model, OS version, uptime, etc.)

Automated configuration backups executed in parallel

Persistent storage of device data and backups using SQLite

REST API for querying collected device information

Designed to support both mock data (early development) and live device connections

Structured logging and error handling for connection and execution failures

**Current state**
Initial version used mocked Netmiko responses for UI and data flow testing

Current version connects to Nokia practice servers and performs real SSH sessions

**Planned enhancements**
Execute show commands against live devices (e.g., DevNet sandbox)

Capture and store structured command output

Export results as TXT and JSON

Full per-session logging for auditability and troubleshooting


### Ansible Network Automation Demo

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
