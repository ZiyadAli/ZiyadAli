- 👋 Hi, I’m @ZiyadAli
- 👀 I’m interested in MVC .Net Core
- 🌱 I’m currently learning Angular
- 💞️ I’m looking to collaborate on !
- 📫 How to reach me ...

<!---
ZiyadAli/ZiyadAli is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.

--->
 Set and reset proxy for git and npm connection
Depending on whether the connection is behind a proxy or not, the proxy settings will need to set/reset correspondingly when using npm and git.

The command to set  the proxy are

# Set proxy for npm:
npm config set proxy http://proxy:8080
npm config set https-proxy http://proxy:8080

# Set proxy for git:
git config --global http.proxy http://proxy:8080
git config --global https.proxy http://proxy:8080


The command to reset proxy for npm 
npm config rm proxy
npm config rm https-proxy


# reset proxy for git
git config --global --unset http.proxy
git config --global --unset https.proxy

# get proxy setting for git
git config --global --list
npm config get list
npm config get proxy
npm config get https-proxy


The command to set proxy for windows 8.1 command line terminal
Set proxy for all apps from terminal
netsh winhttp set proxy proxy:8083

Reset proxy for all apps from terminal
netsh winhttp reset proxy

Show proxy settings
netsh winhttp show proxy

Set proxy for windows 
in pc settings, go to network->prxoy settings to change the proxy settings.
