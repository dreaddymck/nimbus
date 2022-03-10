# nimbus
Repo for nimbus - a tool for controling jailbroken iDevices from SSH. Activator needed to work properly.
INSTALLING: Download the nimbus file and place it to /usr/bin by using iFILE or Filza file manager.
Controlling: type "nimbus help" in the on-device terminal emulator or from SSH for a list of commands.

# nimbus_dmck
Override default menu items by sourcing a .nimbus script located in the home directory.
Override example code :

```bash
#!/bin/bash
example_action_function(){
    #...
}
# required function
nimbus_custom_menu(){
    printf "%$((${COLLUMN0} + ${COLLUMN1}))s\n" " " | tr ' ' '-'
    printf "%-${COLLUMN0}s %-${COLLUMN1}s\n" "example_action_function "example menu description"
}

```
