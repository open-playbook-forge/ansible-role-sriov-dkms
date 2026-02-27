# SRIOV-DKMS

Ansible role for installing the i915 SR-IOV DKMS module on Proxmox VE hypervisors and Debian hosts:
https://github.com/strongtz/i915-sriov-dkms

## Prerequisites

Set the following kernel command-line arguments on the target hypervisor host(s): `intel_iommu=on iommu=pt`.

In addition, the Python requirements for this role have to be installed on the Ansible controller:

```bash
pip3 install -r requirements.txt
```

# Warnings

The i915 SR-IOV DKMS module is *highly experimental* and not ready for production use.

This role will reboot your machine if changes are detected. To prevent this and reboot manually, set the following variable either in your inventory, your playbook or the command-line:

```yaml
auto_reboot: false
```
