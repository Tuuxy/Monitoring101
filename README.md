Dozens of Linux server system monitoring commands are built into the operating system.
Including the likes of *top* or *sar*. Or you can also use monitoring programs such as *glance* , *htop* or *Netdata*.

Four Linux system monitoring tools are important to learn in details : 

#### [[Sar]]

System Activity Reporter (sar) is part of the [Sysstat system resource utilities package](https://github.com/sysstat/sysstat). Sar is a do-it-all monitoring tool. It measures CPU activity; memory/paging; interrupts; device load; network; process and thread allocation; and swap space utilization. Sar can be used interactively, but its real value is that it keeps data logs over a long period of time, which you can use to troubleshoot recurring problems and produce reports. To learn more, read our [How to Use the System Activity Reporter (sar)](https://www.linode.com/docs/guides/how-to-use-sar) guide.


#### [[Vmstat]]

This virtual memory statistics reporter is a built-in Linux command-line tool. In addition to reporting in detail on virtual memory usage, vmstat also gathers information on memory usage, memory paging, processes, I/O, CPU, and storage scheduling. Unlike sar, vmstat starts on boot. It’s used to report on cumulative activity since the last reboot. Our [Use vmstat to Monitor System Performance](https://www.linode.com/docs/guides/use-vmstat-to-monitor-system-performance) guide includes more information about getting started with this monitoring tool.


#### [[Monitorix]]

Monitorix is a free, open-source tool that monitors multiple Linux services and system resources. Monitorix, from version 3.0 on, comes with its own web server. This makes it useful for remote Linux system monitoring. Originally designed for the [Red Hat Enterprise Linux (RHEL)](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux) operating system family, Monitorix now works on all major Linux server distributions. Read our [How to use Monitorix for System Monitoring](https://www.linode.com/docs/guides/how-to-use-monitorix-for-system-monitoring) guide to learn more.


#### [[Nethogs]]

This free and open-source program extends the net top tool that tracks bandwidth by process. For example, you might discern that the amount of outbound traffic has increased on your Linux server, but Nethogs helps you identify which process is generating the usage spikes. Other network monitoring utilities only break down the traffic by protocol or subnet. Read our [Get Started Using Nethogs for Network Usage Monitoring](https://www.linode.com/docs/guides/get-started-using-nethogs-for-network-usage-monitoring) guide to learn more about this tool.

Why using Linux system monitoring programs ? 
To make sure that :

- The hardware is working.
- The server is up and running.
- The server resources are sufficient for mission-critical applications and services to work at peak performance.
- No resource bottlenecks are slowing things down.
- System administrators are alerted when a KPI fails to meet its specified metric.
- Data is presented in a visual manner – such as dashboards, graphs, and weather maps — to visualize trends that aren’t obvious in raw data.

These programs do this by tracking:

- The server’s real-time status
- Data collected over time to enable analysis of long-term trends.
- Data collected to determine the best use of server resources for mission-critical applications. For example, does [InnoDB](https://en.wikipedia.org/wiki/InnoDB) or [MyISAM](https://en.wikipedia.org/wiki/MyISAM) work best for the database storage engine?

Specifically, Linux system monitors look at:

- Memory usage
- CPU usage
- Storage usage, including disk space and Input/Output Operations per Second (IOPS)
- Network usage



-- WIP