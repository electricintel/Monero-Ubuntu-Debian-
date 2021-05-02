# Monero-Ubuntu-Debian- from https://techexpert.tips/monero/installing-monero-node-linux/

Tutorial - Monero Node Installation

Use the following commands to install the required libraries:

# apt-get install libboost-all-dev

Download the Monero installation package.

# mkdir /downloads
# cd /downloads
# wget https://downloads.getmonero.org/linux64

If the above wget doesn't work, download the copy from this repository and move it to /downloads, then extract and install it with the below instructions

Extract and install the Monero node software.

# tar -jxvf linux64
# cd monero-v0.11.1.0/
# install -sv monerod monero-wallet-cli /usr/local/bin/
# install -sv monero-wallet-rpc monero-blockchain-export /usr/local/bin/
# install -sv monero-blockchain-import /usr/local/bin/

Start the Monero node using the following command:

# monerod

Wait for the synchronization of the blockchain to end.

The blockchain synchronization might take days or weeks.

Use the following command to verify the status of the blockchain synchronization:

# tail -f ~/.bitmonero/bitmonero.log


