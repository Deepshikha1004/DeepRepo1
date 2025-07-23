# SOP Documentation: Creating a Virtual RHEL Server for Web Application Testing    


## 1. Title
**Creating a Virtual RHEL Server for Web Application Testing**

---

## 2. Purpose
This SOP outlines the process of creating a virtual server using Red Hat Enterprise Linux (RHEL) to test web applications. It ensures that the environment is secure, isolated, and closely resembles a production setup for realistic application testing.

---

## 3. Scope and Objectives
The scope of this SOP includes the setup and configuration of a virtual RHEL server to perform web application testing.

**Objectives:**
- Install a virtual RHEL server using VirtualBox or KVM.
- Configure the LAMP stack (Linux, Apache, MariaDB, PHP).
- Set up networking and security (firewall, SELinux).
- Deploy and test a sample web application.
- Ensure the server can be reused and easily restored via snapshots.

---

## 4. Accountability Matrix

| Objective                      | Responsible Personnel  |
|-------------------------------|------------------------|
| Install virtual RHEL server   | System Administrator   |
| Configure LAMP stack          | System Administrator   |
| Network and security setup    | Network Administrator  |
| Web application deployment    | Web Developer          |
| Snapshot and backup           | System Administrator   |

---

## 5. Reversion Information

| Version | Date       | Changes Made                                     |
|---------|------------|--------------------------------------------------|
| 1.0     | 2025-07-16 | Initial version created for SOP documentation.  |
| 1.1     | 2025-07-17 | Updated steps and accountability roles.         |

---

## 6. Steps

1. Download and install VirtualBox or KVM on the host system.
2. Create a new virtual machine and mount the RHEL ISO image.
3. Follow the installation wizard to install RHEL on the VM.
4. Configure system network settings (static IP, DNS).
5. Update all packages using DNF (`dnf update -y`).
6. Install Apache, MariaDB, and PHP using DNF.
7. Configure the firewall to allow HTTP and HTTPS traffic.
8. Verify SELinux policies and adjust if necessary.
9. Deploy a sample web application and test connectivity.
10. Create a VM snapshot for rollback purposes.

---

## 7. Approval Table

| Name        | Role               | Date Approved |
|-------------|--------------------|----------------|
| John Smith  | IT Manager         | 2025-07-16     |
| Jane Doe    | Project Supervisor | 2025-07-16     |

---

