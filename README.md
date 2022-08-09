# my-series-IV-rust-near-blockchain-part-1  
  
https://github.com/elicorrales/blockchain-tutorials/blob/main/How-To-Set-Up-Env-Common.md  
  
```
sudo apt update && sudo apt -y upgrade
```
  
```
rustup update
```
  
```
rustup target add wasm32-unknown-unknown
```
  
```
cargo build --target wasm32-unknown-unknown --release
```
  
```
sudo apt install python3 python3-pip python3-dev
```
```
pip3 --version
```
```
pip 20.0.2 from /usr/lib/python3/dist-packages/pip (python 3.8)
```
  
```
pip3 install --upgrade pip
```
```
usr/lib/python3/dist-packages/secretstorage/util.py:19: CryptographyDeprecationWarning: int_from_bytes is deprecated, use int.from_bytes instead
  from cryptography.utils import int_from_bytes
/home/IamDeveloper/.local/lib/python3.8/site-packages/cryptography/hazmat/backends/openssl/x509.py:14: CryptographyDeprecationWarning: This version of cryptography contains a temporary pyOpenSSL fallback path. Upgrade pyOpenSSL now.
  warnings.warn(
Collecting pip
  Downloading pip-22.2.2-py3-none-any.whl (2.0 MB)
     |████████████████████████████████| 2.0 MB 2.1 MB/s
Installing collected packages: pip
Successfully installed pip-22.2.2
```
  
```
npm install -g near-cli
```
  
```
near login
```
  
It opens up a browser
```
Please authorize NEAR CLI on at least one of your accounts.

If your browser doesn't automatically open, please visit this URL
https://wallet.testnet.near.org/login/?referrer=NEAR+CLI&public_key=ed25519%3ACSR4DuZNS5dMchmd7ZpUa1wRUtjLNxnu7K68KFNyRHrv&success_url=http%3A%2F%2F127.0.0.1%3A5000
Please authorize at least one account at the URL above.

Which account did you authorize for use with NEAR CLI?
Enter it here (if not redirected automatically):
Logged in as [ mynearlocalwallet.testnet ] with public key [ ed25519:CSR4Du... ] successfully

IamDeveloper@SoftwareDevelopUbuntu2004  (main)
~/GitHub/my-series-IV-rust-near-blockchain-part-1
$
```
  
We go into more detail in the Part 3 video of : [Series I - NEAR Blockchain Tutorial](https://github.com/elicorrales/blockchain-tutorials/blob/main/README.md#series-i---near-blockchain-tutorial-deploying-wasm)  
Here is [the Part 3 video](https://www.youtube.com/watch?v=8gPVbUc5Zos&list=PLNKa8O7lX-w5Myr19mn-dxtSphB5X1jUW&index=4)  
  
```
near state mynearlocalwallet.testnet
```
```
Account mynearlocalwallet.testnet
{
  amount: '199999875105225000000000000',
  block_hash: 'HmvP4WPgdZ5yLj22k5PP1eyty7xU1E2fAMDgq3RNTPC2',
  block_height: 97105136,
  code_hash: '11111111111111111111111111111111',
  locked: '0',
  storage_paid_at: 0,
  storage_usage: 428,
  formattedAmount: '199.999875105225'
}
```
  
Perhaps either create an Bash ```alias```, or a global ```export```.  I chose an alias.  
In ```~/.bashrc```, near bottom, I added:  
```
alias localnear="NEAR_ENV=localnet;near";
```
  
The above distinguishes the command I would run when deploying to local node vs deploying to testnet.  
  

```
localnear deploy --accountId mynearlocalwallet.testnet --wasmFile target/wasm32-unknown-unknown/release/rust-counter-tutorial-bin-lib.wasm
```


