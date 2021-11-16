# Test Vagrant

Testing how to use Vagrant with VirtualBox.

Creates a single VM and installs Docker and Kubernetes.

## Run

```bash
vagrant up
```

Kubernetes dashboard should be available at `https://192.168.1.180:3000'

Admin token for logging into the dashboard will be output into the `token` file.