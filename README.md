# grid-vsc

https://code.visualstudio.com/docs/remote/faq

Can VS Code Server be installed or used on its own?#
No. The VS Code Server is a component of the Remote Development extensions and is managed by a VS Code client. It is installed and updated automatically by VS Code when it connects to an endpoint and if installed separately could become quickly out of date. It is not intended or licensed for use by other clients.




https://code.visualstudio.com/docs/setup/linux

```
wget -qO- https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > packages.microsoft.gpg
sudo install -o root -g root -m 644 packages.microsoft.gpg /etc/apt/trusted.gpg.d/
sudo sh -c 'echo "deb [arch=amd64,arm64,armhf signed-by=/etc/apt/trusted.gpg.d/packages.microsoft.gpg] https://packages.microsoft.com/repos/code stable main" > /etc/apt/sources.list.d/vscode.list'
rm -f packages.microsoft.gpg
```
Then update the package cache and install the package using:
```
sudo apt install apt-transport-https
sudo apt update
sudo apt install code # or code-insiders
```


VSC Command Line Interface (CLI)
https://code.visualstudio.com/docs/editor/command-line


install python
