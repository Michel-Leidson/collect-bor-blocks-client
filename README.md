# Blocks Monitoring
 
-------
1 - Download .deb file
###
```
wget https://github.com/Michel-Leidson/collect-bor-blocks-client.git/releases/download/1.0.2/sp-tools-cbbc_1.0.2_amd64.deb
```
Install
--------
```
sudo dpkg -i sp-tools-cbbc_1.0.2_amd64.deb
```
2 - Configure the your Signer Address
###
```
sudo nano /etc/cbbc/config
```
3 - Restart service
###
```
sudo systemctl restart cbbc
```
4 - Enable service
###
```
sudo systemctl enable cbbc
```
5 - Clean up
###
```
rm sp-tools-cbbc_1.0.2_amd64.deb
```
You can monitor the service using journalctl 
###
```
journalctl -u cbbc -f
```
