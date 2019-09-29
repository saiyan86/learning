### Pretty print json in terminal with less:
```
cat X.json | jq . -C | less -r
```

### Grep output from strace
strace progname 2>&1 | grep ...
