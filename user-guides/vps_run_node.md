{% include disclaimer.html translated="no" translationOutdated="no" %}

# havend

`havend` is the @daemon software that ships with the Haven tree. It is a console program, and manages the blockchain. While a bitcoin wallet manages both an account and the blockchain, Haven separates these: `havend` handles the blockchain, and `haven-wallet-cli` handles the account.

This guide assumes you have already set up your VPS account and are using SSH to tunnel into the server console.

## Linux, 64-bit (Ubuntu 16.04 LTS)

### Make sure that port 18080 is open
`havend` uses this port to communicate with other nodes on the Haven network.

Example if using `ufw`: `sudo ufw allow 18080`
Example if using `iptables`: `sudo iptables -A INPUT -p tcp --dport 18080 -j ACCEPT`

### Download the current Haven Core binaries

    wget https://downloads.gethaven.org/linux64

### Make a directory and extract the files.

    mkdir haven
    tar -xjvf linux64 -C haven

### Launch the daemon

    cd haven
    ./havend

### Options:

Show list of all options and settings:

    ./havend --help

Launch the daemon as a background process:

    ./havend --detach

Monitor the output of `havend` if running as daemon:

    tail -f ~/.bithaven/bithaven.log

Keep the VPS secure with autoupdate:

https://help.ubuntu.com/community/AutomaticSecurityUpdates


