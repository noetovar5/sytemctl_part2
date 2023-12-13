<img align="right" src="https://visitor-badge.laobi.icu/badge?page_id=noetovar5.sytemctl_part2"/>
# sytemctl_part2
the second part of learning the systemctl command

`systemctl` is a powerful command in Linux used for controlling the systemd system and service manager. It allows you to manage services, examine their status, start or stop them, 
enable or disable them at system boot, and much more. 
# Here are some commonly used `systemctl` commands and their functionalities:

1. **Start a service:**
   ```bash
   systemctl start service_name
   ```
   This command starts a specified service immediately.

2. **Stop a service:**
   ```bash
   systemctl stop service_name
   ```
   It stops a specified service immediately.

3. **Restart a service:**
   ```bash
   systemctl restart service_name
   ```
   It stops and then starts a service again.

4. **Enable a service at boot:**
   ```bash
   systemctl enable service_name
   ```
   This command configures a service to start automatically during system boot.

5. **Disable a service at boot:**
   ```bash
   systemctl disable service_name
   ```
   It stops a service from starting automatically during system boot.

6. **Check the status of a service:**
   ```bash
   systemctl status service_name
   ```
   This command shows the current status of a service, including whether it's running, stopped, or encountering errors.

7. **Check all active units:**
   ```bash
   systemctl list-units --type=service
   ```
   This command displays a list of all active services on the system.

8. **Reload systemd configuration changes:**
   ```bash
   systemctl daemon-reload
   ```
   Use this command after making changes to unit files (service definitions) to reload the systemd manager configuration.

9. **View service logs:**
   ```bash
   journalctl -u service_name
   ```
   This command shows logs specific to a particular service.

10. **Mask or unmask a service:**
    ```bash
    systemctl mask service_name
    systemctl unmask service_name
    ```
    Masking a service prevents it from being started manually or by other services. Unmasking reverses this action.

These commands can be used by system administrators to effectively manage services and system behavior in a Linux environment controlled by systemd. 
Always ensure you have the necessary permissions (often sudo or root access) to execute these commands, as some operations may require elevated privileges.
