# linux
Linux Basics
Linux Directory Structure
Linux follows the Filesystem Hierarchy Standard (FHS). The root (/) is the starting point, and everything else branches out from it.
Here are the main directories and their purposes:
1. /
	• Root directory – the top-level directory.
	• Everything (files, directories, devices) starts here.

2. /bin
	• Essential user binaries (commands) needed for booting and basic operation.
	• Example: ls, cat, cp, mv, bash.

3. /sbin
	• System binaries (programs for system administration).
	• Example: shutdown, mount, ifconfig.

4. /boot
	• Files needed for booting Linux.
	• Contains the kernel (vmlinuz), initramfs, and GRUB bootloader configs.

5. /dev
	• Device files (everything in Linux is treated as a file).
	• Example: /dev/sda (disk), /dev/tty (terminal).

6. /etc
	• System-wide configuration files.
	• Example: /etc/passwd (user accounts), /etc/ssh/sshd_config.

7. /home
	• User home directories.
	• Example: /home/alice, /home/bob.
	• Each user stores personal files, configs, and data here.

8. /lib, /lib64
	• Shared libraries required by programs in /bin and /sbin.
	• Equivalent to DLLs in Windows.

9. /media
	• Mount points for removable media like USB drives, CDs.

10. /mnt
	• Temporary mount point for manually mounting filesystems.

11. /opt
	• Optional software (third-party applications not part of base system).
	• Example: Google Chrome, VMware tools.

12. /proc
	• Virtual filesystem that provides kernel and process information.
	• Example: /proc/cpuinfo, /proc/meminfo.

13. /root
	• Home directory of the root user (superuser).

14. /run
	• Stores runtime data (process IDs, sockets). Cleared on reboot.

15. /srv
	• Service data for servers (web, FTP, etc.).

16. /sys
	• Virtual filesystem containing kernel info about devices.

17. /tmp
	• Temporary files.
	• Cleared on reboot or periodically.

18. /usr
	• User applications and files.
	• Contains the bulk of Linux software.
		○ /usr/bin → Non-essential binaries (editors, compilers).
		○ /usr/sbin → Non-essential system binaries.
		○ /usr/lib → Libraries.
		○ /usr/local → Locally installed software.

19. /var
	• Variable data (changes frequently).
	• Example: logs (/var/log/), caches, mail, spool files.

✅ In short:
	• /bin, /sbin → Core commands
	• /etc → Config
	• /home → User data
	• /var → Logs, caches, temp data
	• /boot → Bootloader + kernel
	• /proc, /sys → Virtual kernel info
	• /usr → Applications and libraries

