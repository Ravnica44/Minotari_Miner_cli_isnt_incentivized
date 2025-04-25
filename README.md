```shell
cd $HOME && adduser --gecos "" tari && usermod -aG sudo tari
```

```shell
su - tari
```

```shell
sudo apt update
sudo apt install automake libtool protobuf-compiler libudev-dev -y
```

```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
```

```shell
echo 'export PATH="$HOME/.cargo/bin:$PATH"' >> ~/.bashrc && source ~/.bashrc
```

```shell
git clone https://github.com/tari-project/tari.git
cd ~/tari && TARI_NETWORK=nextnet TARI_TARGET_NETWORK=nextnet cargo build --release
```

```shell
screen -S tari_node
```


./target/release/minotari_node

Initializing logging according to "/home/layeredge/.tari/esmeralda/config/base_node/log4rs.yml"
Node config does not exist.
Would you like to mine (Y/n)?
NOTE: this will enable additional gRPC methods that could be used to monitor and submit blocks from this node.

ENTER

Node identity does not exist.
Would you like to create one (Y/n)?

ENTER



./target/release/minotari_console_wallet

Console Wallet

1. Create a new wallet.
2. Recover wallet from seed words or hardware device.
3. Create a read-only wallet using a view key.
>> 1
Create wallet passphrase:
Confirm wallet passphrase:

Would you like to use a connected hardware wallet? (Supported types: Ledger) (Y/n)
n
Apr 24 22:33:33.490 [warn] Fixing permissions on directory /home/layeredge/.tari/esmeralda/libtor/wallet/data

=========================
       IMPORTANT!
=========================
These are your wallet seed words.
They can be used to recover your wallet and funds.
WRITE THEM DOWN OR COPY THEM NOW. THIS IS YOUR ONLY CHANCE TO DO SO.

=========================
scare promote interest word lunch neglect frozen laundry possible reduce vintage snake fashion acid rifle cute arrange faint gain same strike machine achieve slam
=========================

I confirm that I will never see these seed words again.
Type the word "confirm" to continue.
>> confirm


Local Base Node detected with public key 207959d61608817132aba05c28cff4384960dcfb1274953d62f00a50f130bf2b and address /onion3/z2w644qooeic3wzg3dsnztcg3obyv7xumoe2ue6lzed6lckzn2yue5yd:18141
Would you like to use this base node? IF YOU DID NOT START THIS BASE NODE YOU SHOULD SELECT NO (Y/n)

ENTER

Please enter 'wallet-payment-address' ('quit' or 'exit' to quit) : f2HUv2XmUx5G6m26PbXGYknBK8jGkVJHCeZ9Ueuiox6N3Frt7bq1ULMFY67a3WKZVyXEFFQQCaiRQdcVjWS5GD5Zbb6
Please enter 'base-node-grpc-address' ('quit' or 'exit' to quit) : http://127.0.0.1:18142
22:45 INFO  👛 Connecting to base node at http://127.0.0.1:18142
22:45 INFO  ⛏ Miner 05 reported 0.07MH/s with total 1.13MH/s over 16 threads. Height: 519. Target: 6244203114)
22:45 INFO  ⛏ Miner 13 reported 0.08MH/s with total 1.31MH/s over 16 threads. Height: 519. Target: 6244203114)
22:45 INFO  ⛏ Miner 10 reported 0.10MH/s with total 1.67MH/s over 16 threads. Height: 519. Target: 6244203114)
22:45 INFO  ⛏ Miner 15 reported 0.10MH/s with total 1.59MH/s over 16 threads. Height: 519. Target: 6244203114)
22:45 INFO  ⛏ Miner 01 reported 0.08MH/s with total 1.32MH/s over 16 threads. Height: 519. Target: 6244203114)



./target/release/minotari_miner

Update

cd ~/tari
git fetch
git checkout main
git pull
cargo build --release
