# SEND Masternode
### Bash installer for SEND Masternode on Ubuntu 16.04 LTS x64

#### This shell script comes with 4 cronjobs: 
1. Make sure SEND daemon is always running: `makerun.sh`
2. Make sure SEND daemon is never stuck: `checkdaemon.sh`
3. Make sure SEND daemon is always up-to-date: `upgrade.sh`
4. Clear the log file every other day: `clearlog.sh`

#### This is just to copy the pre-compiled daemon. Login to your vps as root, download the install_sendmn.sh file and then run it. Note: This will reboot the server.
```
wget https://raw.githubusercontent.com/CannaBitss/send_masternode/master/installmn.sh
bash ./installmn.sh
```

#### If you just want to install without dependencies, Login to your vps as root, download the install_sendmn_nodeps.sh file and then run it. Note: This will NOT reboot the server, use this only when you already have dependencies installed.
```
wget https://raw.githubusercontent.com/CannaBitss/send_masternode/master/install_sendmn_nodeps.sh
bash ./install_sendmn_nodeps.sh
```

#### To compile the daemon from source code. Login to your vps as root, download the install_sendmn_compile.sh file and then run it. Note: This will reboot the server.
```
wget https://raw.githubusercontent.com/CannaBitss/send_masternode/master/install_sendmn_compile.sh
bash ./install_sendmn_compile.sh
```


#### On the client-side, add the following line to masternode.conf: Masternode Private Key should be aligned between the wallet controller and VPS Wallet
```
node-alias vps-ip:50050	node-key collateral-txid vout
```

#### Run the qt wallet, go to Masternode tab, choose your node and click "start alias" at the bottom.

#### Masternode Setup Guide:
```

```
