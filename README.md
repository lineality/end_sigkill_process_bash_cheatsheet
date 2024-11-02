#### end_sigkill_process_bash_cheatsheet

# Kill Process

## To see what process is active [bash]
```bash
$ sudo nethogs
$ top
```
In Top:
- type 'h'
- Kill process: Scroll with arrows until your target process is at the top of the list. Type 'k'. 

## End process by <processID>(PID) with:
- https://github.com/lineality/find_pid_listening_at_port

### List what processes are listening at port (user your port number below)
```bash
sudo lsof -n -i :8080 | grep LISTEN
```
or
```bash
sudo lsof -n -i :5555
```
#### Example output: In this example '12345' is the process-ID (PID)
```
python3 12345 username    4u  IPv4 645737      0t0  TCP 127.0.0.1:rfe (LISTEN)
```


## End process by <processID>(PID) with:
```bash
$ kill -9 <processID>(PID)
```
or
```bash
$ kill -SIGKILL <processID>(PID)
```
#### For Example:
```bash
$ kill -SIGKILL 12345
```

