# install_kubeadm

Installs kubeadm, kubelet, kubectl.

## Role Variables

```yaml
install_kubeadm_kubernetes_version: v1.29.2 # Version of kubernetes. Be warned updating this value will not upgrade a kubernetes cluster.
install_kubeadm_disable_selinux: true # Flag to indicate if selinux system should be disabled. Default: true
```

## Example Playbook

    - hosts: servers
      roles:
         - { role: wittdennis.install_kubeadm, install_kubeadm_kubernetes_version: v1.29.2 }

## License

MIT
