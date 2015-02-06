# SSH

## Tunnel

### Local
Use remote services through local port
```
ssh -L [local-port]:[host]:[host-port] [user]@[host]
```

### Remote
Use local services through remote port
```
ssh -R [local-port]:[host]:[host-port] [user]@[host]
```

### Useful flags
- **-f** go to background just before command execution
- **-N** do not execute a command on the remote system

## Links
- http://blog.trackets.com/2014/05/17/ssh-tunnel-local-and-remote-port-forwarding-explained-with-examples.html
