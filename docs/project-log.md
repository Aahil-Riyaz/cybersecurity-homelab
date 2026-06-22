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

1. Install Ubuntu Server 26.04
2. Configure networking and SSH access
3. Update the system packages
4. Install Docker
5. Deploy Pi-hole
6. Configure firewall and security settings
## Day 2

Successfully installed Ubuntu Server 26.04 on the Lenovo laptop.

Configured Wi-Fi networking, enabled OpenSSH for remote access, and updated the system packages.

Installed Docker and verified the installation using the hello-world container.

Attempted a native Pi-hole installation, which became unresponsive during package installation. As a result, I decided to deploy Pi-hole using Docker containers instead.

### Progress

- Ubuntu Server installed
- Wi-Fi configured
- OpenSSH enabled
- System updated
- Docker installed and tested
- Began Pi-hole deployment using Docker
