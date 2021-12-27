# Ansible Execution Environment

### Build execution environment
`ansible-builder build --tag=ansible-ee --container-runtime podman`

### Tag with Private Automation Hub IP
`podman tag localhost/ansible-ee XX.XX.XX.XX/ansible-ee`

### Publish on Private Automation Hub
`podman push --tls-verify=false --remove-signatures XX.XX.XX.XX/ansible-ee`