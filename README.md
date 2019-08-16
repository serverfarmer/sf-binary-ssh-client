sf-binary-ssh-client is a dependency extension, providing OpenSSH 6.7
client. It is provided for compatibility reason, since OpenSSH 7
deprecated several old encryption algorithms, that are still in use
by various network equipment, and other specialized devices.

It also provides a simple wrapper script, which automatically detects
current OS version and architecture, and executes the proper ssh binary.

On older systems, native system version is used instead of provided one,
eg. to avoid problems with AppArmor/SELinux/whatever is used to enhance
system security.
