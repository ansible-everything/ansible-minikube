# Ansible role minikube

Configure minikube cluster

## Requirements

* Ansible >= 2.9 (Earlier versions may work, but I haven't tested)

## Role Variables

All variables in [default/main.yml](defaults/main.yml) can be overrided

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
|`minikube_driver`| docker | minikube [driver options](https://minikube.sigs.k8s.io/docs/drivers/)|

## Dependencies

Nil

## Example Playbook

This role is not released in galaxy yet to utilze this role, you can add this repo as a git submodule

```bash
git submodule add -b main https://github.com/slashpai/ansible-minikube.git roles/minikube
```

```yaml
- hosts: all
  roles:
    -minikube
```

To get role updates

```bash
git submodule update --remote
```

## Contributing

**TODO:** To be updated

## License

[MIT](LICENSE)
