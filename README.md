# dotfiles
Custom Dot Files that I like to use

# Installation
## basic apps
`apt install git vim curl`

## [VS Code](https://code.visualstudio.com/docs/setup/linux)
```curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'
```
```
sudo apt-get update
sudo apt-get install code
```

## NVM
`curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash`

## [yarn](https://yarnpkg.com/en/docs/install#debian-stable)
```
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo apt-get install --no-install-recommends yarn
```

## global packages
### [prettier](https://prettier.io)
`yarn global add prettier`

### Create React (Native) App
`yarn global add create-react-app create-react-native-app`

### [commitizen](https://github.com/commitizen/cz-cli)
```
yarn global add commitizen cz-emoji

# set as default adapter for your projects
echo '{ "path": "cz-emoji" }' > ~/.czrc
```

### [gren](https://github.com/github-tools/github-release-notes)
```
yarn global add github-release-notes
echo 'export GREN_GITHUB_TOKEN=yourPersonalAccessTokenHere' > ~/.bash_profile
```
