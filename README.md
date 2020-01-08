# proc_notify
## Monitor linux proc events
### Requires
* CONFIG_PROC_EVENTS=y

### Usage
- **wait_events** - receive events
- **start_listen** - start listening. This can be called inside a callback to enable listening after a disconnect
- **disconnect** - disconnect. This can be called inside a callback to disconnect before starting a long operation. If not disconnected notifications will continue to be queued
- **stop_event_loop** - exit the event loop. This can be called inside a callback to tell the loop to exit and return control.
- **disconnect** - closes the connection
