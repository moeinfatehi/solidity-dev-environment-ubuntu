# Setup Solidity Smart Contract Development Environment on Ubuntu 22

## Install Ganache UI on Ubuntu:
* Download appimage from <a href="https://trufflesuite.com/docs/ganache/">here (trufflesuite ganache project page)</a></br>
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
