#FireWall
1. It's possible to show service status of firewall like folows. (enabled by default)
[root@asus]systemctl status firewalld
[root@asus]#systemctl stop firewalld
[root@asus]#systemctl disable firewalld
#SELinux
2. It's possible to show Status of SELinux(Security-Enhandced Linux) like follows (endabled by default)
[root@asus]#getenforce
3. If SELinux function does not need for you because of some reasons like that your server is running only in Local safety Network or others, it's possbile to disable it like follows.
[root@asus]#vi /etc/selinux/config
SELINUX=disabled	change to disabled

restart to apply new setting
[root@asus]#reboot
