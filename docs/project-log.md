# Project Log

## Day 1

I found an old Lenovo laptop that was no longer being used and decided to repurpose it as a cybersecurity home lab.

The goal of this project is to gain hands-on experience with Linux administration, networking, Docker, self-hosted services, and cybersecurity tools.

### Progress

* Created the GitHub repository for the project
* Documented the laptop hardware specifications
* Planned the homelab architecture and future services
* Downloaded the Ubuntu Server 26.04 ISO
* Created a bootable USB drive using Rufus
* Prepared the laptop for Ubuntu Server installation

### Notes

The bootable USB was successfully created and verified. The next step is to boot the laptop from the USB drive and install Ubuntu Server.

### Planned Next Steps

* Install Ubuntu Server 26.04
* Configure networking and SSH access
* Update the system packages
* Install Docker
* Deploy Pi-hole
* Configure firewall and security settings

---

## Day 2

Successfully installed Ubuntu Server 26.04 on the Lenovo laptop.

Configured Wi-Fi networking, enabled OpenSSH for remote access, and updated the system packages.

Installed Docker and verified the installation using the hello-world container.

Attempted a native Pi-hole installation, which became unresponsive during package installation. As a result, I decided to deploy Pi-hole using Docker instead.

During deployment, Docker reported that port 53 was already in use by Ubuntu's systemd-resolved service. After troubleshooting the issue and freeing the port, I successfully launched the Pi-hole container.
Successfully deployed Pi-hole using Docker.

The initial Pi-hole installation method became unresponsive, so I switched to a Docker-based deployment.

During setup I encountered a port conflict on port 53 caused by systemd-resolved. After troubleshooting the issue, I reconfigured the system and successfully launched the Pi-hole container.

The container is running correctly and passed its health checks.

Successfully accessed the Pi-hole web dashboard and verified that the container was running correctly.

The dashboard loaded successfully with the default blocklists, showing over 82,000 blocked domains available for filtering.

This confirmed that Docker networking, container deployment, and web access were functioning correctly.

### Additional Progress

* Accessed the Pi-hole dashboard from a web browser
* Verified successful Docker container deployment
* Confirmed Pi-hole services were running correctly
* Verified default blocklists were loaded
* Completed initial Pi-hole setup

Progress
Pi-hole deployed with Docker
Container health verified
Docker networking troubleshooting completed

Lessons Learned
Docker container deployment
Port conflict troubleshooting
Linux networking services
Basic container management


### Progress

* Ubuntu Server installed
* Wi-Fi configured
* OpenSSH enabled
* System updated
* Docker installed and tested
* Pi-hole image downloaded
* Troubleshot Docker networking issues
* Successfully deployed Pi-hole using Docker
* Verified that the Pi-hole container is running

### Lessons Learned

* How to create a bootable USB using Rufus
* Basic Ubuntu Server installation and configuration
* Using SSH for remote management
* Installing and testing Docker containers
* Troubleshooting port conflicts in Linux
* Deploying services using Docker

### Next Steps

* Access the Pi-hole web dashboard
* Configure devices to use Pi-hole as their DNS server
* Install and configure UFW Firewall
* Set up Tailscale for remote access
* Deploy additional Docker services
* Begin security hardening of the server
