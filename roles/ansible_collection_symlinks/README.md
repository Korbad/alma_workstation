# Symlink Playbook

---
- hosts: localhost
  tasks:
  - include_tasks: tasks/symlink-collection.yml
    vars:
      collection_namespace: korbad
      collection_name: alma_workstation
      github_org: Korbad
      github_repo: alma_workstation
  - include_tasks: tasks/symlink-collection.yml
    vars:
      collection_namespace: korbad
      collection_name: docker_manager
      github_org: Korbad
      github_repo: docker_manager
