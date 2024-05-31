# Ansible Automation Platform configuration as code (CaC)

**Red Hat Communities of Practice Controller Configuration Collection**
- [infra.controller_configuration Documentation]( https://console.redhat.com/ansible/automation-hub/repo/validated/infra/controller_configuration/docs/ "infra.controller_configuration Documentation")

**You will need the infrastructure as code to use this experimental feature**
- [Using postinstall feature of containerized Ansible Automation Platform]( https://access.redhat.com/documentation/en-us/red_hat_ansible_automation_platform/2.4/html/containerized_ansible_automation_platform_installation_guide/aap-containerized-installation#using-postinstall_aap-containerized-installation "Using postinstall feature of containerized Ansible Automation Platform")
- [aws_ansible_deployment_containerized gitrepo]( https://github.com/ericcames/aws_ansible_deployment_containerized "aws_ansible_deployment_containerized gitrepo")

**Red Hat Ansible Automation Hub configuration as code (CaC)**
- [aap.automation_hub.config CaC]( https://github.com/ericcames/aap.automation_hub.config "aap.automation_hub.config CaC")

Example excerpt from inventory file:
===========
```
# AAP Controller - optional
# -------------------------
# To use the postinstall feature you need to set these variables
controller_postinstall=true
controller_license_file=/home/ansible-svc/.manifest/{{ manifest_file_name }}
controller_postinstall_dir=/home/ansible-svc/git-repos
# When using config-as-code in a git repository
controller_postinstall_repo_url={{ controller_postinstall_repo_url }}
controller_postinstall_repo_ref=main
```