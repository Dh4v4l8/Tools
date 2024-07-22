# Tools

## PDTM 
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
```
