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

```shell
cd tari
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
cd tari
./target/release/minotari_console_wallet
```

navigate with ➜ en go to "Receive" then copy your `Tari Address one-sided`

`Ctrl` + `A` + `D`

```shell
screen -S tari_miner
```

```shell
cd tari
```

```shell
./target/release/minotari_miner
```

Update

cd ~/tari
git fetch
git checkout main
git pull
cargo build --release
