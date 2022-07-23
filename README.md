# Setup Solidity Smart Contract Development Environment on Ubuntu 22

## Install Ganache UI on Ubuntu:
Quickly fire up a personal Ethereum blockchain which you can use to run tests, execute commands, and inspect state while controlling how the chain operates.
* Download the latest version of appimage from <a href="https://trufflesuite.com/docs/ganache/">here (trufflesuite ganache project page)</a></br>
* Add execution permission to the downloaded file:</br>
  `chmod +x ganache-*.AppImage`
* Before running, make sure that libfuse2 is installed.</br>
  `sudo apt-get install libfuse2`
* Run Ganache UI:</br>
`./ganache-*.AppImage`

## Install SOLC (The Solidity Compiler) on Ubuntu:
###### Using apt-get:
`sudo add-apt-repository ppa:ethereum/ethereum`</br>
`sudo apt-get update`</br>
`sudo apt-get install solc`</br>
* Make sure solc is installed by getting the solc version:</br>
`solc --version`</br>
Output:</br>
`solc, the solidity compiler commandline interface`</br>
`Version: 0.8.15+commit.e14f2714.Linux.g++`

###### Using snap:
`sudo snap install solc`</br>
* Make sure solc is installed by getting the solc version:</br>
`solc --version`</br>
* This version may be lower than the version of the installed package from apt-get.

Reference: https://docs.soliditylang.org/en/latest/installing-solidity.html

## Install Truffle on Ubuntu:
A world class development environment, testing framework and asset pipeline for blockchains using the Ethereum Virtual Machine (EVM), aiming to make life as a developer easier. </br>
* Make sure that "npm" is installed.</br>
`sudo apt-get install npm`
* Install truffle using npm:</br>
`sudo npm install -g truffle`
* Make sure solc is installed by getting the truffle version:</br>
`truffle version`</br>
