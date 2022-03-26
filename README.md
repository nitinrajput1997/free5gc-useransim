# free5gc-useransim

### Setup free5gc
##### Install NodeJs and yarn
```bash
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update
sudo apt-get install -y nodejs yarn
```
##### Build WebConsole
```bash
git clone https://github.com/free5gc/free5gc.git
cd ~/free5gc
make webconsole
```
##### Using WebConsole to Add an UE
First start up the WebConsole server:
```bash
cd ~/free5gc/webconsole
go run server.go
```
**Note:** The screen shows the port number :5000 at the end. Open your web browser from your host machine, and enter the URL http://192.168.5.93:5000
On the login page, enter username admin and password free5gc
Once logged in, widen the page until you see “Subscribers” on the left-hand side column.
Choose Subscribers and create a new data:
Note that other than the “Operator Code Type” field which you should choose “OP” for now, leave other fields unchanged. This registration data is used for ease of testing and actual use later.
After the data is created successfully, you can press Ctrl-C on the terminal to quit WebConsole.

#####
