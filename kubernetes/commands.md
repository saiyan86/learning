### Get client certificate data from kubeconfig (client-certificate from kubeconfig)
```
export client=$(grep client-cert ~/.kube/config |cut -d" " -f 6)
```
This is used by curl to use the specified client certificate when getting a file with HTTPS, FTPS or another SSL-based  protocol.
### Get private key data from kubeconfig (client-key from kubeconfig)
```
export key=$(grep client-key-data ~/.kube/config |cut -d " " -f 6)
```
This is the private key used by curl.
### Get CA key data from kubeconfig (certificate-authority from kubeconfig)
```
export auth=$(grep certificate-authority-data ~/.kube/config |cut -d " " -f 6)
```
This is used by curl to use the specified certificate to verify the peer.
### Set file ownership
```
sudo chown $(id -u):$(id -g) $HOME/.kube/config
```
