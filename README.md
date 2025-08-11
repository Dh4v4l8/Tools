# Tools
## kali speedup
```
sudo cd /etc/apt/
cat sources.list (replace http with https in the second link)
sudo apt install apt-transport-https
sudo apt upgrade
```

## [PDTM](https://github.com/projectdiscovery/pdtm)
```
sudo apt update
sudo apt upgrade
```
```
sudo apt install golang-go
echo $PATH
go env | grep GOPATH   (GOPATH='/home/kali/go')
nano .zshrc
export PATH="$PATH:/home/kali/go/bin"
source .zshrc
echo $PATH
```
```
go install -v github.com/projectdiscovery/pdtm/cmd/pdtm@latest
pdtm -ia
sudo rm /usr/bin/httpx
```
## [assetfinder](https://github.com/tomnomnom/assetfinder)
```
sudo apt install git
git --version
sudo git clone https://github.com/tomnomnom/assetfinder.git
go mod init assetfinder
go build .
sudo mv assetfinder /usr/local/bin/
assetfinder
```
## [httprobe](https://github.com/tomnomnom/httprobe)
## [waybackurls](https://github.com/tomnomnom/waybackurls/tree/master)
## [waymore](https://github.com/xnl-h4ck3r/waymore)
```
Installation is straightforward:

git clone https://github.com/xnl-h4ck3r/waymore.git
cd waymore
sudo python setup.py install
sudo pip3 install -r requirements.txt
```
## [gau](https://github.com/lc/gau)
## [gauplus](https://github.com/bp0lr/gauplus)
## [gospider](https://github.com/jaeles-project/gospider)
## [hakrawler](https://github.com/hakluke/hakrawler)
## [ParamSpider](https://github.com/devanshbatham/ParamSpider)

## [kiterunner](https://github.com/assetnote/kiterunner/releases)

```
tar xf kiterunner_1.0.2_linux_amd64.tar.gz 
sudo mv kr /opt/kr
sudo ln -s /opt/kr /usr/local/bin/kr
kr
```
## [LinkFinder](https://github.com/GerbenJavado/LinkFinder)
## [SecretFinder](https://github.com/m4ll0k/SecretFinder)
## [nowafpls](https://github.com/m4ll0k/nowafpls)
