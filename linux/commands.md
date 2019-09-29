### Pretty print json in terminal with less:
```
cat X.json | jq . -C | less -r
```

### Grep output from strace
```
strace X 2>&1 | grep ...
```
