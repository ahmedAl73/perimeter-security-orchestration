# perimeter-security-orchestration
Firewall configuration, ingress control, and validation on Linux systems

# Perimeter Security Orchestration & Ingress Control

## Executive Summary
This project demonstrates the configuration, enforcement, and validation of perimeter security controls on a Linux system. The objective is to implement firewall rules that regulate ingress traffic, verify that legitimate traffic is permitted, and confirm that unauthorized traffic is blocked. The work emphasizes operational accuracy, troubleshooting, and verifiable evidence rather than task completion alone.

---

## Environment
- **Operating System:** Linux (Fedora / Ubuntu)
- **Firewall Technology:** firewalld
- **Tools & Utilities:** firewall-cmd, systemctl, journalctl
- **Access Method:** Local terminal and SSH

---

## Objective
The primary goal of this project is to design and enforce perimeter security controls that:
- Restrict unauthorized inbound network traffic
- Allow explicitly permitted services
- Persist across system reboots
- Provide verifiable evidence of correct enforcement

---

## Validation & Verification
System behavior was validated using multiple verification steps:
- Active firewall rules were inspected to confirm correct configuration
- Authorized traffic was tested and confirmed to pass successfully
- Unauthorized traffic was tested and confirmed to be blocked
- System logs were reviewed to validate enforcement behavior

Screenshots and command output demonstrating successful validation are stored in the `/proof` directory.

---

## Diagnostics & Corrective Learning
During implementation, configuration issues were encountered related to rule application order and service definitions. These issues were diagnosed by reviewing firewall status output and system logs, then corrected by adjusting rule scope and reloading the firewall configuration.

Detailed error descriptions, root causes, and corrective actions are documented in the `/diagnostics` directory.

---

## Translation Note (Training → Industry)
This project was originally completed as a firewall configuration lab. It has been reframed and documented using industry-standard terminology and practices to reflect professional security engineering work.

**Original training context:** Firewall lab exercise  
**Professional framing:** Perimeter Security Orchestration & Ingress Control

---

## Repository Structure
