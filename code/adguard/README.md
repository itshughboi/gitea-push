# To-do
Think about how to fully secure this with DoH or DoT so that upstream ISP's or networks can't even see what domain I'm going to
Might be beneficial to route public queries through vpn for anonymity? Could be slow and detrimental to performance



### Installation
1. Remove stub listener on linux host
```sh
sudo nano /etc/systemd/resolved.conf
```
^^ Uncomment DNSStubListener=yes & set the value to 'no'
```
sudo systemctl restart systemd-resolved
```
