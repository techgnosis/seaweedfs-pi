Use Ubuntu. Raspberry Pi OS just does not work well.

I did not modify the Ubuntu image at all. 

Username and password are `ubuntu:ubuntu`

Unit file was installed into `/etc/systemd/system`

Then `sudo systemctl enable seaweedfs`

Then `sudo systemctl start seaweedfs`

Access Filer at port `8888`


wget https://github.com/seaweedfs/seaweedfs/releases/download/3.23/linux_arm64.tar.gz

wget https://github.com/grafana/agent/releases/download/v0.26.1/agent-linux-arm64.zip


Use `weed mount` to mount the whole remote file tree as a local folder. Easier to manage folders this way.

Use `weed benchmark` to test against the master server and see your performance


### TECH DEBT
1. It's possible that the unit files should go in `/etc/systemd/user` instead of `/etc/systemd/system` since the process runs as a non-root user and it's managing data owned by a non-root user
