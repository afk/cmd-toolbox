# SSH

## Tunnel
```
ssh -f [user]@[host] -L [local-port]:[host]:[host-port] -N
```
**-f** go to background just before command execution;
**-N** do not execute a command on the remote system
