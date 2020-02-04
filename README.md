# zramctl-meminfo

Short and simple bash script displaying memory usage stats for ZRAM on Ubuntu. It wraps calls to Ubuntu's `zramctl` and the kernel's `/proc/meminfo`to display the following:

```
RAM Addressable      15.4G
    Used              9.6G
    Not Compressed    9.2G
    Compressed      357.2M
    Uncompressed    850.6M

Effective RAM Used   10.1G
Compression Ratio      2.4
```

To use this script first enable ZRAM by installing and starting the following service (the second command saves having to reboot):

```bash
sudo apt install zram-config
sudo service zram-config start
```

