
### What is Sar ? 

**Sar** stands for **System Activity Reporter**. It is a command-line utility for collecting, reporting, and analyzing system activity data on Linux systems. Sar is a part of the **Sysstat package**, which provides various system performance monitoring tools.

Sar gathers data on various system resources and activities, including CPU utilization, memory usage, disk I/O, network traffic, and more. It collects this data at regular intervals and stores it for later analysis. This historical data can be invaluable for diagnosing performance issues, identifying trends, and optimizing system resources.

### How to install Sar ?

Install package :

```
sudo apt-get install sysstat
```

Enable sar in /etc/default/sysstat configuration file : 

```
ENABLE="true"
```

Default configurations work but if you want to change them, they are located in :

```
sudo cat /etc/cron.d/sysstat
sudo cat /etc/sysstatsysstat
```

By default, the `debian-sa1` script runs every 10 minutes and collects sar data for historical reference. This data is written to the `/var/log/sysstat/saXX` file, where `XX` is the day of the month. For example, if today is the 24th day of the month, `sa1` writes the sar data to `/var/log/sysstat/sa24`. To change the logging frequency to one minute, change `5-55/10` to `5-55/1`. To make it 2 minutes, change it to `5/55/2`, and so on.
### How to use Sar ? 

The syntax to use sar is : 

```
sudo sar [option] -f /path/to/sar/file
```

If no sar file is specified it will display the current day sar file

![Sar Current Day](/Assets/sar_default.png)

Linux 6.8.4-200.fc39.x86_64 is the kernel version.
(fedora) is the hostname.
x86_64 is the system architecture.
(4 CPU) is the number of CPU cores available.

You can use man sar to delve into the possible options to use with sar.





























