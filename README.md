# riptutorial

  CentOS broken repositories fix:  
```
  $ cd /etc/yum.repos.d/    
  $ sed -i 's/mirrorlist/#mirrorlist/g' /etc/yum.repos.d/CentOS-*  
  $ sed -i 's|#baseurl=http://mirror.centos.org|baseurl=http://vault.centos.org|g' /etc/yum.repos.d/CentOS-*
```
  (replace the existed Baseurl with the vault.centos.org)  
  
# RHEL
```
$ yum install -y yum-utils
$ yum-config-manager --add-repo https://download.docker.com/linux/rhel/docker-ce.repo
$
$ yum install iputils procps net-tools pip tree netcat crontab jq
```
  
# pcap  
Get files from S3 (local name test2.txt required)  
```
aws s3 cp s3://mybucket/test.pcap test2.pcap
```
    
# JavaScript, self invoking function definition  
```
(function diy(x){setTimeout(diy, 1000, x+1); console.log("counting: ", x)})(1)
```
(function definition in parenasis + argument)  
- or -
```
function diy(){setTimeout(diy, 1000); console.log(Date.now())}
diy()
```


