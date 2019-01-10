# catbrokers4
Set up OLM managed Service Catalog, Ansible Broker and Template Broker on an existing OpenShift 4 cluster

- Tested against libvirt cluster created by OpenShift 4 installer v0.9.1 https://github.com/openshift/installer/releases/tag/v0.9.1

## Usage
1. Set up an OpenShift 4.0 cluster
1. Wait for all cluster components to come up, since the playbook will scale down the Cluster Version Operator (CVO)
1. Login to the cluster by setting `KUBECONFIG` environment variable or using `oc login`
1. Start the playbook with `./run-playbook.sh`
