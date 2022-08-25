Use Ubuntu. Raspberry Pi OS just does not work well.

I did not modify the Ubuntu image at all. 

Username and password are `ubuntu:ubuntu`

Unit file was installed into `/etc/systemd/system`

Then `sudo systemctl enable seaweedfs`

Then `sudo systemctl start seaweedfs`

Access Filer at port `8888`