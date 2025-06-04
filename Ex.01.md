
# EXP NO : 1 Create a Repository
### AIM:
To create a repository.
### PROCEDURE:
1. SSH login
The first line shows an SSH login to a server with the IP address 172.25.250.11. The user logging in
is root . SSH (Secure Shell) is a network protocol that allows secure remote login to a server. The
root user is the system administrator account and has full access to all commands and files on the
system.
2. Enabling the web console
The next line shows a command to acHvate the web console with systemctl enable-now
cockpit.socket. Cockpit is a web-based interface for managing Linux systems. Enabling the socket
tells the system to start the Cockpit service whenever the system boots.
3. Registering with Red Hat Insights
The line insights-client-register registers the system with Red Hat Insights. Red Hat Insights is a
subscripHon service that provides system health reports and recommendaHons for security and
performance improvements.
4. Viewing Yum repositories
The user then edits the file /etc/yum.repos.d/local.repo using the vi text editor. Yum is a package
manager for Red Hat-based systems. Repos (repositories) are locaHons where soRware packages
are stored. The local.repo file likely contains configuraHon informaHon for custom yum
repositories.
5. Checking Yum repository informaHon
ARer ediHng the file, the user uses the cat command to view the contents of /etc/yum.repos.d/
local.repo. The cat command is used to display the contents of a file.
6. Cleaning Yum packages
The next command is dnf clean all. Dnf is a newer version of yum that is used in Red Hat Enterprise
Linux 8 and later. The clean all command removes cached package metadata.
7. LisHng Yum repositories
The user then uses the dnf repolist all command to list all configured repositories. The output
shows two repositories configured: appstream and baseos. These are the default repositories for
Red Hat Enterprise Linux 9.
8. Installing Vim
The final command is dnf install vim -y. This command installs the Vim text editor using the dnf
package manager. The -y flag tells dnf to assume yes to all prompts, which is useful for una[ended
installaHons.

### OUTPUT:
![image](https://github.com/user-attachments/assets/e686fd54-2e20-49a9-bc53-142b6be7b477)

### RESULT:
Thus a repository has been created successfully.
