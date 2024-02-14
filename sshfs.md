# sshfs


SSHFS is a FUSE-based filesystem client for mounting remote directories over a Secure Shell connection. 


In order to be able to mount a directory the SSH user needs to be able to access it. Invoke sshfs to mount a remote directory: 

```bash
sshfs [user@]host:[dir] mountpoint [options]

```