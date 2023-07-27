```bash
sudo ifconfig
```
- Used to identify the interfaces that are available.
- The Ethernet network interface is identified by the entry with the ```eth``` prefix.

</br>
</br>

```bash
sudo tcpdump -D
```
- Also used to identify the interfaces that are available

</br>
</br>

```bash
sudo tcpdump [-i interface] [option(s)] [expression(s)]
```
- The ```-i``` parameter specifies the network interface to capture network traffic. 
- The ```option(s)``` are optional and provide you with the ability to alter the execution of the command.
  - ```-w``` used to write or save the sniffed network packets to a packet capture file.
  - ```-r``` used to read a packet capture file by specifying the file name.
  - ```-v``` | ```-vv``` | ```-vvv``` used to control how much packet information you want tcpdump to print out.
  - ```-c``` lets you control how many packets tcpdump will capture.
  - ```-n``` disables this automatic mapping of numbers to names and
    - considered to be best practice when sniffing or analyzing traffic. 
    - ```-n``` will not resolve hostnames
    - ```-nn``` will not resolve both hostnames or ports
- The ```expression(s)``` are a way to further filter network traffic packets so that you can isolate network traffic.

>Note: You can combine options together. For example, -v and -n can be combined as -vn. But, if an option accepts a parameter right after it like -c 1 or -r capture.pcap then you can’t combine other options to it.