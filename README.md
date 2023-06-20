# NoSleep.sh

## Bash Script to Edit `/etc/systemd/logind.conf`

This bash script is designed to edit the `/etc/systemd/logind.conf` configuration file on a Rocky Linux Server or Workstation. Specifically, it modifies the `HandleLidSwitch` option and sets it to `ignore`. This configuration change is commonly used to prevent the system from suspending or performing any action when the laptop lid is closed.

### Usage

To use the script, follow these steps:

1.  Open a terminal on your Linux system.
2.  Save the provided script into a file, for example, `edit_logind_conf.sh`.
3.  Make the script executable by running the command `chmod +x edit_logind_conf.sh`.
4.  Execute the script as root using the command `sudo ./edit_logind_conf.sh`.
5.  The script will update the `HandleLidSwitch` option in the `logind.conf` file to `ignore`.
6.  Optionally, you will be prompted to reboot the system for the changes to take effect immediately.

### Important Notes

* This script **must** be run as root or with superuser privileges to modify system files.
* It assumes that the `logind.conf` file is located at `/etc/systemd/logind.conf`. If your system uses a different location, please modify the script accordingly.
* Modifying system configuration files can have unintended consequences. Please review the changes made by the script and ensure they align with your requirements.
* It's recommended to take appropriate precautions, such as backing up the original configuration file, before executing the script.
* Rebooting the system is optional but can ensure that the changes take effect immediately. You will be prompted to reboot after executing the script.

---

Feel free to customize and use the script according to your needs. Please ensure that you understand the script and its implications before running it on your system.
