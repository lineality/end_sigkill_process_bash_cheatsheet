# end_sigkill_process_bash_cheatsheet

# Kill Process

To see what process is active [bash]
```bash
	$ sudo nethogs
	$ top
```

End process by <processID>(PID) with:
```bash
$ kill -9 <processID>(PID)

Or

$ kill -SIGKILL <processID>(PID)
```
