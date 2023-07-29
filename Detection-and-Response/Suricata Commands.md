### Run Suricata on packet capture example:
```bash
sudo suricata -r sample.pcap -S custom.rules -k none
```
>Notes:
The -r sample.pcap option specifies an input file to mimic network traffic. In this case, the sample.pcap file.
The -S custom.rules option instructs Suricata to use the rules defined in the custom.rules file.
The -k none option instructs Suricata to disable all checksum checks.

</br>
</br>

### Log output example:
```
alert http $HOME_NET any -> $EXTERNAL_NET any (msg:"GET on wire"; flow:established,to_server; content:"GET"; http_method; sid:12345; rev:3;)
```
> - ```alert``` represents action part, it also can be ```drop```, ```pass```, and ```reject```.
> - ```http $HOME_NET any -> $EXTERNAL_NET any``` represents header part, ```http``` represents protocol used, ```$HOME_NET``` represents source IP address, ```$EXTERNAL_NET``` represents destination IP address, and ```any``` represents port numbers for source and destination.
> - ```(msg:"BAD USER-AGENT";flow:established,to_server;content:!”Mozilla/5.0”; http_user_agent; sid: 12365; rev:1;)``` represents rule options.
    - The ```msg:``` option provides the alert text. In this case, the alert will print out the text “GET on wire”, which specifies why the alert was triggered.
    - The ```flow:established,to_server``` option determines that packets from the client to the server should be matched. (In this instance, a server is defined as the device responding to the initial SYN packet with a SYN-ACK packet.)
    - The ```content:"GET"``` option tells Suricata to look for the word GET in the content of the http.method portion of the packet.
    - The ```sid:12345 (signature ID)``` option is a unique numerical value that identifies the rule.
    - The ```rev:3``` option indicates the signature's revision which is used to identify the signature's   version. Here, the revision version is 3.

</br>
</br>

> Note: You can run eve.json iles using ```jq eve.json | less```