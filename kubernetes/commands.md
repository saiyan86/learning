### Get key data from .crt file
```
export client=$(cat x.crt | cut -d " " -f 6)
```
### Get key data from .key file
```
export client=$(sudo cat x.key | cut -d " " -f 6)
```
### Set file ownership
```
sudo chown $(id -u):$(id -g) $HOME/.kube/config
```
