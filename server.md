# Processes

## Basic commands

```bash
ps -ef # show all processes -e for all and -f for formatted
ps -eo pid= # only show pid (ppid= to show parent id)
pwdx pid # to show current directory of a process
pstree pid # to show tree of a process
```

## Combind commands

```bash
ps -eo pid= | xargs pwdx # to show directory of all processes
ps -ef | grep '\-bash' # leading dash(-) means the command has been run from a login shell
ps -ef | grep 'sleep' # to find sleep commands
```

# Services

## Linux

```bash
journalctl -u service_name -f # tail -f logs of a service
```
