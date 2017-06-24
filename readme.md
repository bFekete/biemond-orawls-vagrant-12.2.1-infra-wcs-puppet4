#WebLogic 12.2.1 webcenter sites 

## Details
- CentOS 7 vagrant box
- Puppet 4
- Vagrant >= 1.8
- Oracle Virtualbox >= 5

Download & Add the all the Oracle binaries to /software

edit Vagrantfile and update the software share to your own local folder
- wlsdb.vm.synced_folder "/Users/edwin/software", "/software"
- wcsadmin.vm.synced_folder "/Users/edwin/software", "/software"

Vagrant boxes
- vagrant up wlsdb
- vagrant up wcsadmin

## Database
- wlsdb 10.10.10.5 with Welcome01 as password

###software
- Oracle Database 12.1.0.2 SE Linux
- linuxamd64_12102_database_se2_1of2.zip
- linuxamd64_12102_database_se2_2of2.zip

## Middleware

### Cluster with 1 node
- wcsadmin 10.10.10.21, WebLogic 12.2.1 with WCS requires RCU

http://10.10.10.21:7001/em with weblogic1 as password

###software
- JDK 1.8u121 jdk-8u121-linux-x64.tar.gz
- JDK 8 JCE policy jce_policy-8.zip
- fmw_12.2.1.2.0_infrastructure.jar
- fmw_12.2.1.2.0_wcsites_Disk1_1of1.zip
