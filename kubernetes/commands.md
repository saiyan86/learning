### Get key data from .crt file
```
export client=$(cat x.crt | cut -d " " -f 6)
```
### Set file ownership
```
sudo chown $(id -u):$(id -g) $HOME/.kube/config
```
