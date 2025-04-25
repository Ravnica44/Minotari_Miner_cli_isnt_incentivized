```shell
cd $HOME && adduser --gecos "" tari && usermod -aG sudo tari
```

```shell
su - tari
```

```shell
sudo apt update
sudo apt install screen automake libtool protobuf-compiler libudev-dev -y
```

```shell
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y
```

```shell
echo 'export PATH="$HOME/.cargo/bin:$PATH"' >> ~/.bashrc && source ~/.bashrc
```

https://github.com/tari-project/tari/blob/development/docs/src/branching_releases.md

```shell
git clone https://github.com/tari-project/tari.git
cd ~/tari && git checkout v1.15.0-rc.0
```

```shell
TARI_NETWORK=nextnet TARI_TARGET_NETWORK=nextnet cargo build --release
```

```shell
screen -S tari_node
```

```shell
cd ~/tari
```

```shell
./target/release/minotari_node
```

WAIT FULL SYNC https://explore-nextnet.tari.com/

`Ctrl` + `A` + `D`

```shell
screen -S tari_wallet
```

```shell
cd ~/tari
./target/release/minotari_console_wallet
```

navigate with ➜ en go to "Receive" then copy your `Tari Address one-sided`

`Ctrl` + `A` + `D`

```shell
screen -S tari_miner
```

```shell
cd ~/tari
```

```shell
./target/release/minotari_miner
```

Past your address `Tari Address one-sided` is `'wallet-payment-address'`
