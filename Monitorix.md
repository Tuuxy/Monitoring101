
### What is Monitorix ?

As per the [Monitorix Website](https://www.monitorix.org): 

**Monitorix is a free, open source, lightweight system monitoring tool** designed to monitor as many services and system resources as possible. It has been created to be used under **production Linux/UNIX servers**, but due to its simplicity and small size can be used on **embedded devices** as well.

It consists mainly of two programs: a collector, called `monitorix`, which is a Perl daemon that is started automatically like any other system service, and a CGI script called `monitorix.cgi`. Monitorix includes its own HTTP server built in (which is listening by default on port 8080/TCP) to see the statistics graphs, so you aren't forced to install a third-party web server to use it. Just point your browser at `http://localhost:8080/monitorix`.

All of its development was initially created for monitoring Red Hat, Fedora and CentOS Linux systems, so this project was made keeping in mind these type of distributions. Today it runs on different GNU/Linux distributions and even in other UNIX systems like FreeBSD, OpenBSD and NetBSD.

It is currently in active development adding new features, new graphs and correcting bugs in the attempt to offer a great tool for daily systems administration.

Monitorix is an open source project and, just like any other open source project, anyone can contribute with his own time and knowledge.

### How to install Monitorix ?

Install package :

```
sudo apt-get install monitorix
```

Either use the default config or change it on : 

```
/etc/monitorix/monitorix.conf
```

After that you can restart the monitorix service :

```
sudo systemctl enable monitorix
sudo service monitorix restart
```

### How to use Monitorix ?

Access it via your browser :

```
http://ipaddress:8080/monitorix
```

![Monitorix Landing Page](/Assets/monitorix_landing.png)

Select All graphs or a particular graph and a time period and click ok :

![Monitorix Graphs ](/Assets/monitorix_graphs.png)


Monitorix can keep track of system load, kernel usage, filesystem usage, network traffic, netstat traffic and many more things.
