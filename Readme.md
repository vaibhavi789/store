#Commands to Run Ansible playbook:

*********** This command is to Deploy/Rollback code on store Application Stack. Please change the environment name and release version accordingly ************

/releases/ansible/venv/bin/./ansible-playbook -i store-inventory  store.yml --tags=stoptomcat,repodownload,copyrepo,explodewar,symlinks,starttomcat -e store_release_version=<> -e target_env=<> --ask-become-pass
