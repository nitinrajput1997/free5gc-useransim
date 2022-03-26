# free5gc-useransim

### Setup free5gc
##### Install NodeJs and yarn
```bash
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update
sudo apt-get install -y nodejs yarn
```
##### build WebConsole
```bash
git clone https://github.com/free5gc/free5gc.git
cd ~/free5gc
make webconsole
```
#####
