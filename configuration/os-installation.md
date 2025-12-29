
# Operating System Installation and Configuration

This document outlines the operating system installation and initial configuration process performed after system assembly and BIOS validation.

---

## 1. Installation Media Preparation

- Created bootable USB installation media using the official Windows Media Creation Tool
- Verified installation media integrity prior to use

---

## 2. OS Installation

- Booted system from USB installation media
- Initiated a clean installation on the NVMe SSD
- Removed existing partitions and allowed the installer to create required system partitions

### Network Driver Limitation and Workaround

During Windows Setup, a network connection (Ethernet or WiFi) was required to continue the installation process. The onboard WiFi adapter was not recognized at this stage, and the manufacturer-provided WiFi driver stored on USB was not accessible through the Windows Setup interface.

To proceed with installation, the following Windows Out-of-Box Experience (OOBE) workaround was applied:

- Opened Command Prompt using `Shift + F10`
- Executed the following command: oobe\bypassnro
- System rebooted and provided the option to continue setup without an internet connection
- Selected **“I don’t have internet”** and completed installation using a local user account

This approach allowed access to the desktop environment, where driver installation from removable media is fully supported.

---

## 3. Initial System Configuration

- Completed initial Windows setup and local account creation
- Verified successful login and desktop load
- Confirmed correct time zone, language, and regional settings
- Verified display output using integrated graphics

---

## 4. Driver Installation and Network Configuration

- Installed chipset and motherboard-specific drivers from USB
- Installed WiFi driver and verified wireless network connectivity
- Confirmed all critical devices were properly recognized by the operating system

---

## 5. System Updates

- Applied all available Windows updates
- Rebooted system as required to complete update process
- Verified system was fully up to date

---

## 6. Basic Security Configuration

- Verified built-in Windows security features were enabled
- Confirmed firewall status
- Ensured automatic updates were enabled

---

## 7. Validation and Readiness

- Performed multiple system reboots to confirm stability
- Verified storage, memory, and CPU utilization at idle
- Confirmed system readiness for application installation and end-user use

---

## 8. Completion

Operating system installation and configuration completed successfully, and the system was validated as stable and ready for daily use.

