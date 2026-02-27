# SRIOV-DKMS

Ansible role for installing the i915-sriov DKMS module on Proxmox VE hypervisors and Debian hosts:
https://github.com/strongtz/i915-sriov-dkms

## Prerequisites

Set the following kernel commandline arguments: `intel_iommu=on iommu=pt`
