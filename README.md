# Proxmox Packer Builds

This project contains the Packer build configuration and other files for cloud-init ready, minimal Proxmox VM templates.

Current boxes:

* ubuntu2004

## Requirements

* Network and API Access to Proxmox
* ISO on Proxmox
* Packer Variables Configured
* Packer Installed


## Usage

```
packer build -var-file="vars.json" packer.json
```

## Example Output

After a few minutes, you'll see the template was created:

![Alt text](docs/packer_complete.png?raw=true "Successful Build Output")

## Other Notes

Preseed has a weak password, make sure to change and disable password login after launching a VM from the template.