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
pip3 install --user nearup
```
```
Collecting nearup
  Downloading nearup-1.7.0-py3-none-any.whl (21 kB)
Requirement already satisfied: click in /usr/lib/python3/dist-packages (from nearup) (7.0)
Collecting psutil
  Downloading psutil-5.9.1-cp38-cp38-manylinux_2_12_x86_64.manylinux2010_x86_64.manylinux_2_17_x86_64.manylinux2014_x86_64.whl (284 kB)
     |████████████████████████████████| 284 kB 2.9 MB/s
Collecting boto3
  Downloading boto3-1.24.47-py3-none-any.whl (132 kB)
     |████████████████████████████████| 132 kB 14.0 MB/s
Collecting botocore<1.28.0,>=1.27.47
  Downloading botocore-1.27.47-py3-none-any.whl (9.0 MB)
     |████████████████████████████████| 9.0 MB 18.7 MB/s
Collecting s3transfer<0.7.0,>=0.6.0
  Downloading s3transfer-0.6.0-py3-none-any.whl (79 kB)
     |████████████████████████████████| 79 kB 4.5 MB/s
Collecting jmespath<2.0.0,>=0.7.1
  Downloading jmespath-1.0.1-py3-none-any.whl (20 kB)
Collecting python-dateutil<3.0.0,>=2.1
  Downloading python_dateutil-2.8.2-py2.py3-none-any.whl (247 kB)
     |████████████████████████████████| 247 kB 18.8 MB/s
Requirement already satisfied: urllib3<1.27,>=1.25.4 in /usr/lib/python3/dist-packages (from botocore<1.28.0,>=1.27.47->boto3->nearup) (1.25.8)
Requirement already satisfied: six>=1.5 in /usr/lib/python3/dist-packages (from python-dateutil<3.0.0,>=2.1->botocore<1.28.0,>=1.27.47->boto3->nearup) (1.14.0)
Installing collected packages: psutil, python-dateutil, jmespath, botocore, s3transfer, boto3, nearup
Successfully installed boto3-1.24.47 botocore-1.27.47 jmespath-1.0.1 nearup-1.7.0 psutil-5.9.1 python-dateutil-2.8.2 s3transfer-0.6.0
```
```
pip3 install --user --upgrade nearup
```
```
Requirement already up-to-date: nearup in ./.local/lib/python3.8/site-packages (1.7.0)
Requirement already satisfied, skipping upgrade: boto3 in ./.local/lib/python3.8/site-packages (from nearup) (1.24.47)
Requirement already satisfied, skipping upgrade: psutil in ./.local/lib/python3.8/site-packages (from nearup) (5.9.1)
Requirement already satisfied, skipping upgrade: click in /usr/lib/python3/dist-packages (from nearup) (7.0)
Requirement already satisfied, skipping upgrade: botocore<1.28.0,>=1.27.47 in ./.local/lib/python3.8/site-packages (from boto3->nearup) (1.27.47)
Requirement already satisfied, skipping upgrade: jmespath<2.0.0,>=0.7.1 in ./.local/lib/python3.8/site-packages (from boto3->nearup) (1.0.1)
Requirement already satisfied, skipping upgrade: s3transfer<0.7.0,>=0.6.0 in ./.local/lib/python3.8/site-packages (from boto3->nearup) (0.6.0)
Requirement already satisfied, skipping upgrade: python-dateutil<3.0.0,>=2.1 in ./.local/lib/python3.8/site-packages (from botocore<1.28.0,>=1.27.47->boto3->nearup) (2.8.2)
Requirement already satisfied, skipping upgrade: urllib3<1.27,>=1.25.4 in /usr/lib/python3/dist-packages (from botocore<1.28.0,>=1.27.47->boto3->nearup) (1.25.8)
Requirement already satisfied, skipping upgrade: six>=1.5 in /usr/lib/python3/dist-packages (from python-dateutil<3.0.0,>=2.1->botocore<1.28.0,>=1.27.47->boto3->nearup) (1.14.0)
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

https://github.com/near/nearup 
  
Dockerfile:  
```
#ELI changed to ubuntu:20.04
#from ubuntu:20.04
#ELI changed to ubuntu:22.04
from ubuntu:22.04

#original
#from ubuntu:18.04

ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8
ENV PATH="/root/.local/bin:$PATH"
ENV HOME="/root"


#ELI
#RUN apt-get update && apt-get -y upgrade
RUN apt update \
    &&  apt -y upgrade \
    &&  apt install -y file \
    &&  apt install -y net-tools \
    &&  apt install -y vim \
    &&  apt install -y python3 python3-pip \
    &&  pip3 install --upgrade pip


#original
#RUN apt-get update && apt-get install -y python3 python3-pip &&  pip3 install --upgrade pip

COPY . /root/nearup/
RUN cd /root/nearup && pip3 install --user .
COPY ./start.sh /root/start.sh
RUN chmod +x /root/start.sh

#original
#ENTRYPOINT ["/root/start.sh"]

#ELI
#note: even without a CMD bash, running a container with -it drops one into a shell
#because the underlying ubuntu has that binary.
#CMD ["/bin/bash"]
```

```
#ELI changed to ubuntu:20.04
#from ubuntu:20.04
#ELI changed to ubuntu:22.04
from ubuntu:22.04

#original
#from ubuntu:18.04

ENV LANG C.UTF-8
ENV LC_ALL C.UTF-8
ENV PATH="/root/.local/bin:$PATH"
ENV HOME="/root"


#ELI
#RUN apt-get update && apt-get -y upgrade
RUN apt update \
    &&  apt -y upgrade \
    &&  apt install -y file \
    &&  apt install -y net-tools \
    &&  apt install -y vim \
    &&  apt install -y python3 python3-pip \
    &&  pip3 install --upgrade pip


#original
#RUN apt-get update && apt-get install -y python3 python3-pip &&  pip3 install --upgrade pip

COPY . /root/nearup/
RUN cd /root/nearup && pip3 install --user .

COPY ./start.sh /root/start.sh
RUN chmod +x /root/start.sh

#original
#ENTRYPOINT ["/root/start.sh"]

#ELI
#note: even without a CMD bash, running a container with -it drops one into a shell
#because the underlying ubuntu has that binary.
#BUT running a NON-interactive container will cause it to stop because there's nothing to do.
#this is true even if the CMD [.. is NOT commented out
#CMD ["/bin/bash"]

#ELI
#this version has a unlimited loop and it outputs a dot every few secs.
#the trap will catch the listed signals, echo 'shutdown' then exit shell.
#the trap is useful both if you want to stop the container from within, or outside of.

#CMD [ "/bin/bash", "-c", "trap 'echo stopnear;nearup stop;sleep 3;echo shutdown;exit 1;' SIGINT SIGTERM SIGQUIT SIGKILL; while [ 1 ]; do echo -n '.'; sleep 2; done;"]
CMD [ "/bin/bash", "-c", "/root/start.sh"]
```
  
```start.sh```
```
#!/bin/bash
trap 'echo stopnear;nearup stop;sleep 4;echo shutdown;exit 1;' SIGINT SIGTERM SIGQUIT SIGKILL;
echo "$@"
#ELI ELI - modified
#nearup "$@" && while true; do echo -n "."; sleep 3; done;
nearup run localnet && while true; do echo -n "."; sleep 3; done;
```
  

```
sudo docker build . --tag mynearupimg2204:bash
sudo docker build . --tag mynearupimg2204:nobash
```
  
Running interactive containers:
```
sudo docker run -it -v $HOME/.mynearup:/root/.near -p 3030:3030 --name mynearupbash mynearupimg2204:bash
sudo docker run -it -v $HOME/.mynearup:/root/.near -p 3030:3030 --name mynearupnobash mynearupimg2204:nobash
```
  
Either one above drops you into a Bash shell
  
Running non-interactive "bash" or "nobash"(CMD commented out) containers will cause them to stop:  
```
sudo docker run  -v $HOME/.mynearup:/root/.near -p 3030:3030 --name mynearupnobash mynearupimg2204:nobash
sudo docker run  -v $HOME/.mynearup:/root/.near -p 3030:3030 --name mynearupbash mynearupimg2204:bash
```
  
Why? Because there isn't anything for them to keep doing.  Let's prove that.
Add the following to the above Dockerfile: ```CMD ["/bin/bash","-c","while [ 1 ]; do echo -n '.'; sleep 1; done;"]```
```
sudo docker run -v $HOME/.near:/root/.near -p 3030:3030 --name mynearup nearprotocol/nearup run localnet
```

```
sudo docker exec nearup nearup logs
sudo docker exec nearup nearup stop
sudo docker exec nearup nearup run {betanet/testnet}
```
