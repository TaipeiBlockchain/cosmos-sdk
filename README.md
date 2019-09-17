# cosmos-sdk

```bash
apt-get update
apt-get install -y g++ gcc libc6-dev make git curl unzip nano

cd projects
wget https://dl.google.com/go/go1.13.linux-amd64.tar.gz
tar -C /usr/local -xzf go1.13.linux-amd64.tar.gz

echo "export PATH=$PATH:/usr/local/go/bin" >> /etc/profile
source /etc/profile
go version

mkdir -p $HOME/go/bin
echo "export GOPATH=$HOME/go" >> /etc/profile
echo "export GOBIN=\$GOPATH/bin" >> /etc/profile
echo "export PATH=\$PATH:\$GOBIN" >> /etc/profile
echo "export GO111MODULE=on" >> /etc/profile
source /etc/profile

git clone https://github.com/cosmos/sdk-application-tutorial.git
cd sdk-application-tutorial
go mod download
make install
```
