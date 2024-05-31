# Ansible Automation Platform configuration as code (CaC)

**Red Hat Communities of Practice Controller Configuration Collection**
- [infra.controller_configuration Documentation]( https://console.redhat.com/ansible/automation-hub/repo/validated/infra/controller_configuration/docs/ "infra.controller_configuration Documentation")

**You will need the infrastructure as code to use this experimental feature**
- [Using postinstall feature of containerized Ansible Automation Platform]( https://access.redhat.com/documentation/en-us/red_hat_ansible_automation_platform/2.4/html/containerized_ansible_automation_platform_installation_guide/aap-containerized-installation#using-postinstall_aap-containerized-installation "Using postinstall feature of containerized Ansible Automation Platform")
- [aws_ansible_deployment_containerized gitrepo]( https://github.com/ericcames/aws_ansible_deployment_containerized "aws_ansible_deployment_containerized gitrepo")

**Red Hat Ansible Automation Hub Configuration Collection**
- [infra.ah_configruation Documentation]( https://console.redhat.com/ansible/automation-hub/repo/validated/infra/ah_configuration/docs/ "infra.ah_configruation Documentation")

Example excerpt from inventory file:
===========
```
# AAP Controller - optional
# -------------------------
# To use the postinstall feature you need to set these variables
controller_postinstall=true
controller_license_file=/home/ansible-svc/.manifest/manifest_Zigfreed_20240528T153016Z.zip
controller_postinstall_dir=/home/ansible-svc/git-repos
# When using config-as-code in a git repository
controller_postinstall_repo_url=https://github.com/ericcames/aap.controller.config.git
controller_postinstall_repo_ref=main
```