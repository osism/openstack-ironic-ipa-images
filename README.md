# openstack-ironic-ipa-images

## ironic-python-agent-builder

* <https://docs.openstack.org/ironic-python-agent-builder/latest/>
* <https://github.com/openstack/ironic-python-agent-builder>

### Installation

```bash
virtualenv ipa-builder
source ./ipa-builder/bin/activate
pip install diskimage-builder ironic-python-agent-builder

Ubuntu Focal
ironic-python-agent-builder -o ./ipa-ubuntu --release focal -e dynamic-login -e extra-hardware ubuntu

CentOS 8
ironic-python-agent-builder -o ./ipa-centos --release 8 -e dynamic-login -e extra-hardware centos
```

### HPE Proliant Tools

```bash
ironic-python-agent-builder -o ./ipa-ubuntu-proliant --release focal -e dynamic-login -e extra-hardware -e proliant-tools ubuntu
```
