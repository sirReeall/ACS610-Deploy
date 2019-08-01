acs-download
=========

Downloads and extracts Alfresco Content Services 6.1 binaries.

There are no configuration activities preformed in this role.

ACS 6.1 is downloaded from Nexus, this is the Enterprise release and will require a user account and password to be specified when running this role.

You can use Ansible-Vault to create and encrypted password if required, these can be supplied when running the role.

You could also supply the nexus_user and nexus_password via the parent playbook, either via extra_opts (insecure) or var_prompt (require interactive mode)

Role Variables:
---

Installation directory for ACS 6.1
    acs_install_folder: /opt/alfresco

User that will own the acs_install_folder recursively
    alfresco_user: alfresco

Nexus user name:
    nexus_user:

Nexus password (This must be encrypted if you are configuring this):
    nexus_password:
