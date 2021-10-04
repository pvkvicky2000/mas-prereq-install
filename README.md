# mas-prereq-install
Prereq software installation script for Maximo Application Suite 8.4/8.5

Example:
```bash
$ yum install jq gettext git wget
$ git clone --recursive https://github.com/nishi2go/mas-prereq-install
$ cd mas-prereq-install
# Get your key from https://myibm.ibm.com/products-services/containerlibrary
$ export ENTITLEMENT_KEY=<Your entitlement key>
$ export MONGO_REPLICAS=3
# Specify your storage class https://kubernetes.io/docs/concepts/storage/persistent-volumes/
$ export STORAGECLASS_RWO=managed-nfs-storage
$ export STORAGECLASS_RWM=managed-nfs-storage
$ export DOMAIN_NAME=mas.ocp.lan
$ oc login -u maxadmin -p ************ https://api.mas.ocp.lan:6443
$ bash setup.sh
```
