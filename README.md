<b>The contract address:</b> 0x53Ecc62C4Cb327014E1f2007A68B74B3f50B6df3 <br>
<b>Transaction ID:</b> 0x5b07c09dfa934c86ffcec256bc44fd06ab5b560b2e7afe2ddd05b76af6a5408f

<b>Libraries Used:</b>

Truffle:
It is the development environment which uses EVM used to create Dapps much easier. It comes with a boiler plate code so that we can make the developement much more easier.

Web3:
It gives us a collection of libraries that allow us to interact with any local or remote ethereum node.

truffle-hdwallet-provider:
The Truffle HDWallet provider is used to easily configure connections to ethereum. Here we use it to connect with the Rinkeby Public Network.

Solidity: v0.4.24
Node: 12.18.4
Truffle: v4.1.14
web3: v0.20.6
truffle-hdwallet-provider: v1.0.17

<b>Procedure to run</b>

Change directory to ```ud-supply-chain``` folder and install all requisite npm packages (as listed in ```package.json```):

```
cd ud-supply-chain
npm install
```

Launch Ganache:

```
ganache-cli -m "<<mnemonic>>"
```

In a separate terminal window, Compile smart contracts:

```
truffle compile
```

This will create the smart contract artifacts in folder ```build\contracts```.

Migrate smart contracts to the locally running blockchain, ganache-cli:

```
truffle migrate
```

Test smart contracts:

```
truffle test
```

All 10 tests should pass.

In a separate terminal window, launch the DApp:

```
npm run dev
```
