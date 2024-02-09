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
```bash
$ kill -9 <processID>(PID)

Or

$ kill -SIGKILL <processID>(PID)
```
