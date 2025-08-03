# **Octra - Task 03**



**install rust**

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
source $HOME/.cargo/env
```

**build from source**

```bash
git clone https://github.com/octra-labs/ocs01-test.git
```
```
cd ocs01-test
```
```
cargo build --release
```

**setup**

```bash
cp EI/exec_interface.json .
```

**Import Wallet**

```bash
touch wallet.json
```
```
nano wallet.json
```

**Paste the below words with your wallet data:**
```bash
{
  "priv": "private-key-here",
  "addr": "octxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
  "rpc": "https://octra.network"
}
```

Note the change the private key 

save and exit with 

Ctrl + X , Then press Y , then hit Enter button

**run**

```bash
./target/release/ocs01-test
```
