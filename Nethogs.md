
### What is Nethogs ? 

As per the [Nethogs github page](https://github.com/raboof/nethogs :

NetHogs is a small 'net top' tool. Instead of breaking the traffic down per protocol or per subnet, like most tools do, **it groups bandwidth by process**.

NetHogs does not rely on a special kernel module to be loaded. If there's suddenly a lot of network traffic, you can fire up NetHogs and immediately see which PID is causing this. This makes it easy to identify programs that have gone wild and are suddenly taking up your bandwidth.

Since NetHogs heavily relies on `/proc`, most features are only available on Linux. NetHogs can be built on Mac OS X and FreeBSD, but it will only show connections, not processes.

### How to install Nethogs

Clone the github repository : 

```
git clone https://github.com/raboof/nethogs
```

Install dependencies : 

```
sudo apt install gcc-c++ libpcap-devel ncurses-devel
```

Navigate to your nethogs folder  : 

```
cd /path/to/nethogs
make
sudo make install
hash -r
```

And then you can start nethogs :

```
sudo nethogs
```


### How to use Nethogs ?

Nethogs can be used inside a shell or with a GUI ([using nethogs-qt](http://slist.lilotux.net/linux/nethogs-qt/index_en.html) ), the syntax for nethogs is as such : 

```
sudo nethogs [option] [port name]
```

By default, nethogs measures traffic from and to the eth0 interface ( if you are connected via ethernet ) port if no option or port name is specified.

![Nethogs Default](/Assets/nethogs_default.png)

Nethogs can also be used to monitor multiple network ports at once : 

```
sudo nethogs wlp3s0 tun0
```

![Nethogs Multiple Interface](/Assets/nethogs_multiple.png)


You can check the options by using man nethogs : 

![Nethogs Options](/Assets/nethogs_options.png)







































































