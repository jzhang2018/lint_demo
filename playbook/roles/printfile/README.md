This ansible role and playbook it to demonstrate the use of the ansible-lint.

- To run playbook: ansible-playbook playbook/printfile.yml
- Ansible-lint configuration is in .ansible-lint file. For now, it just lists the path of exclusions
- It integrates with GitHub actions. When the action is triggered, it will run the lint
- To run lint locally: ansible-lint playbook/printfile.yml
- The GitHub action is in .github/workflows/ansible-lint_push_pull.yml
  - The action is triggered on push and pull request
  - The email will be sent to the repository owner