Use Ubuntu. Raspberry Pi OS just does not work well.

I did not modify the Ubuntu image at all. 

Username and password are `ubuntu:ubuntu`

Unit file was installed into `/etc/systemd/system`

Then `sudo systemctl enable seaweedfs`

Then `sudo systemctl start seaweedfs`

Access Filer at port `8888`


wget https://github.com/seaweedfs/seaweedfs/releases/download/3.23/linux_arm64.tar.gz

wget https://github.com/grafana/agent/releases/download/v0.26.1/agent-linux-arm64.zip