# nimbus
Repo for nimbus - a tool for controling jailbroken iDevices from SSH. Activator needed to work properly.
INSTALLING: Download the nimbus file and place it to /usr/bin by using iFILE or Filza file manager.
Controlling: type "nimbus help" in the on-device terminal emulator or from SSH for a list of commands.

# nimbus_dmck
Remove clutter and customize the default menu items by adding a _.nimbus_ script to the home directory for source. Create custom actions and/or copy over preferred menu entries

Override example:

```bash
#!/bin/bash
action(){
    #...
}
# required function
nimbus_custom_menu(){
    printf "%$((${COLLUMN0} + ${COLLUMN1}))s\n" " " | tr ' ' '-'
    printf "%-${COLLUMN0}s %-${COLLUMN1}s\n" "unlock" "unlock interface"
    printf "%-${COLLUMN0}s %-${COLLUMN1}s\n" "action "description"
}

```
