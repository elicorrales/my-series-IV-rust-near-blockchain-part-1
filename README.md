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
npm install -g near-cli
```
  
```
near login
```
  
It opens up a browser
```
$ near login

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
  

