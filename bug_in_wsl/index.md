# Some Bugs in WSL2

# Cannot use 'nvidia-smi' command after login wsl via ssh
+ fixed by add `export PATH=/usr/lib/wsl/lib:$PATH` to `PATH`.
# Cannot use 'git clone'
+ reboot it.
# ssh connect error: kex_exchange_identification: read: Connection reset
+ edit `/etc/hosts.allow` add `sshd: ALL`,restart sshd service.
