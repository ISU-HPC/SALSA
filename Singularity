bootstrap: shub
FROM: ISU-HPC/centos7-base

%labels
AUTHOR Yasasvy Nanyam ynanyam@iastate.edu

%post

yum install -y epel-release
yum install -y python2-devel boost boost-devel
yum install -y python-pip
yum install -y git
yum clean all
rm -rf /var/yum/cache

# Install pip package Networkx v 1.1

pip2 --no-cache-dir install networkx==1.1

# SALSA

cd /
git clone https://github.com/machinegun/SALSA.git
cd SALSA
chmod a+x *.py
