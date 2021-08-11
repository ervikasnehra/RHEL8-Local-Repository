# RHEL8-Local-Repository
RPM Package to configure local repository in RHEL 8 / CentOS 8
Please follow this video guide to create RPM package in Fedora based linux distributions.
https://youtu.be/sNDs6AoNmA8
Steps to use the local repository.
1. Connect the ISO image in your machine and mount it on /mnt using below command.
mount /dev/sr0 /mnt
2. Open terminal and download the package in your machine (RHEL8/CentOS8) using this command.
wget https://github.com/ervikasnehra/RHEL8-Local-Repository/blob/main/localrepo-1-0.noarch.rpm
3. Install the package using either of the below commands.
rpm -ivh localrepo-1-0.noarch.rpm
OR
dnf install localrepo-1-0.noarch.rpm
3. 
4. Verify the repository using below command.
dnf repolist all
5. Test the resository to install any package e.g. httpd using below command.
dnf install -y httpd
You are done.
