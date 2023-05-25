# riptutorial

  CentOS broken repositories fix:  
  
  $ cd /etc/yum.repos.d/    
  $ sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*  
  $ sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
  
  (replace the existed Baseurl with the vault.centos.org)  
  
# RHEL
```
$ yum install -y yum-utils
$ yum-config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo
$
$ yum install iputils procps net-tools pip tree netcat crontab jq
```

# pcap  
https://sev2023.github.io/images/traffic.png   
