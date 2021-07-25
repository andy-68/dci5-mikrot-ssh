# dci5-mikrot-ssh

This is a module to allow DCI5 works with Mikrotik switches via ssh protocol.
It have been tested with CRS354-48G-4S+2Q+ RouterOS v6.47.1-6.48.3

HIER

Only one file, mikrot-ssh


BUILDING

Nor reuired, but you need to check Python modules 
paramiko and xml are installed.

RUN

Put mikrot-ssh to /usr/local/mgr5/var/dcihandlers/ (with standard DCI
installation) and restart in's core, the choose "Mikrotik SSH v0.00.002"
will appears in device type selection.
More information about this procedure you may found here:
https://docs.ispsystem.com/dcimanager/developer-section/how-to-add-a-service-handler

In addition to simplest username/password authentification, you may use public key auth
by entering the "-key=path_to_public_key_file" instead of password. If you enter simply
"-key" without path -- the default value "/usr/local/mgr5/var/modules_ssh_keys/keys_dci"
will be used, this path is defined in 10th line of file mikrotik-ssh

TODO

Or not todo ;-) Statistics-related functions.


