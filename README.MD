#kube
#minikube
#install
# Installing Minikube / Kubernetes

### Pre-requisite 
`pacman -S minikube libvirt qemu dnsmasq iptables-nft`

## Permission
`usermod -aG libvirt $(whoami)`
## Procedure
- `sudo systemctl enable libvirtd.service`
- `sudo systemctl start libvirtd.service`
- `minikube config set driver kvm2`
- `minikube start`

## Final
`minikube kubectl get svc` and there should be:
![[Pasted image 20220119095534.png]]
