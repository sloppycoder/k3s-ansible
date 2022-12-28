# Prepare Raspberry PI cluster for installing K3S

Forked from [this repo](https://github.com/k3s-io/k3s-ansible).

Modified to perform the following:

1. removed support for armhf and CentOS
2. download additional binaries used. e.g. k9s, istioctl, helm


```
# install the cluster
ansible-playbook install.yml -i inventory/rack1

# tear down the cluster
ansible-playbook reset.yml -i inventory/rack1

```

