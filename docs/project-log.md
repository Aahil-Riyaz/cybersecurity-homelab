# Project Log

## Day 1

I found an old Lenovo laptop that was no longer being used and decided to repurpose it as a cybersecurity home lab.

The goal of this project is to gain hands-on experience with Linux administration, networking, Docker, self-hosted services, and cybersecurity tools.

### Progress

- Created the GitHub repository for the project
- Documented the laptop hardware specifications
- Planned the homelab architecture and future services
- Downloaded the Ubuntu Server 26.04 ISO
- Created a bootable USB drive using Rufus
- Prepared the laptop for Ubuntu Server installation

### Notes

The bootable USB was successfully created and verified. The next step is to boot the laptop from the USB drive and install Ubuntu Server.

### Planned Next Steps

- Install Ubuntu Server 26.04
- Configure networking and SSH access
- Update the system packages
- Install Docker
- Deploy Pi-hole
- Configure firewall and security settings

---

## Day 2

Successfully installed Ubuntu Server 26.04 on the Lenovo laptop.

Configured Wi-Fi networking, enabled OpenSSH for remote access, and updated the system packages.

Installed Docker and verified the installation using the hello-world container.

Initially attempted a native Pi-hole installation, but the installation became unresponsive during package configuration. To improve reliability and simplify management, I decided to deploy Pi-hole using Docker instead.

During deployment, Docker reported that port 53 was already in use by Ubuntu's systemd-resolved service. After troubleshooting the issue and reconfiguring the system, I successfully launched the Pi-hole container.

The Pi-hole container started successfully, passed its health checks, and the web dashboard became accessible through a browser.

I then verified DNS functionality by configuring a client device to use Pi-hole as its DNS server and confirmed that DNS queries were reaching the dashboard correctly.

To improve security, I configured UFW Firewall and applied a default deny-incoming policy while allowing only the required ports for SSH and Pi-hole.

Finally, I performed basic SSH hardening and verified that the SSH service restarted successfully without any issues.

### Progress

- Ubuntu Server installed
- Wi-Fi configured
- OpenSSH enabled
- System updated
- Docker installed
- Docker tested using hello-world
- Pi-hole image downloaded
- Docker networking issues resolved
- Pi-hole deployed using Docker
- Pi-hole dashboard accessed successfully
- DNS resolution verified through Pi-hole
- UFW Firewall configured
- SSH hardening completed
- All services verified and operational

### Lessons Learned

- Creating bootable USB drives using Rufus
- Ubuntu Server installation and configuration
- Basic Linux system administration
- Managing Linux services using systemctl
- Docker installation and container deployment
- Troubleshooting Docker networking issues
- Resolving Linux port conflicts
- DNS fundamentals and Pi-hole deployment
- Firewall configuration using UFW
- Basic SSH security hardening
- Git and GitHub documentation practices

### Current Environment

- Ubuntu Server 26.04
- OpenSSH
- Docker
- Pi-hole
- UFW Firewall

### Next Steps

- Install Cockpit Server Management
- Configure Tailscale for remote access
- Deploy network monitoring tools
- Install and configure Wazuh
- Host a personal portfolio website
- Continue security hardening of the homelab

---

## Project Status

### Completed

- Ubuntu Server
- Docker
- Pi-hole
- UFW Firewall
- SSH Hardening

### In Progress

- Cockpit
- Tailscale
- Network Monitoring
- Wazuh

### Planned

- Portfolio Website
- Additional Self-Hosted Services
- Advanced Security Monitoring

---

## Day 3

Configured UFW Firewall and applied basic security rules.

Allowed SSH access on port 22 and opened the required ports for Pi-hole DNS and web management.

Enabled the firewall and verified that all required services remained accessible.

Performed basic SSH hardening by reviewing the SSH configuration and verifying that the SSH service restarted successfully.

Installed Cockpit, a web-based Linux server management dashboard, and configured firewall access for remote management.

Successfully accessed the Cockpit dashboard through a web browser and verified access to system monitoring, networking, storage, logs, and services.

### Progress

* UFW Firewall installed and configured
* SSH service verified after hardening
* Cockpit installed
* Cockpit web interface accessible
* System monitoring dashboard operational

### Lessons Learned

* Linux firewall management using UFW
* Managing services with systemctl
* SSH service configuration
* Web-based Linux administration with Cockpit
* Monitoring system resources and services

### Next Steps

* Install Tailscale
* Deploy network monitoring tools
* Install Wazuh
* Configure automatic backups
* Deploy a portfolio website
