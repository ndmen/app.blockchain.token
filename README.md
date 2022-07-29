# app.blockchain.linearvesting

## Description
See video how it works https://youtu.be/VWKwIiYkYVs

A decentralized application to interact with the MyToken, an 18 decimal token with a total supply of 1000.

Token deployer can add Beneficiaries them addresses and amount. The token release schedule will be per second. 
A beneficiary can release only the amount of token vested and releasable.

Release transfers vested and releasable token to the beneficiary who calls it.

Deployed to Rinkeby test network.

Functions:
1. addBenificiar(address address_, uint256 value_) - add Beneficiaries
2. addLinearVesting(uint256 vestingDuration_) - add Linear Vesting
3. getBenificiarTokenVested(uint256 index_) - chek benificiar value
3. claim(uint256 index_) - add claimed value
4. withdraw(uint256 value_) - withdraw claimed value

Deployed address: https://rinkeby.etherscan.io/address/0xe2cdfDAE0144F1AE8396e65c263F1b744771a574

Deployed token: https://rinkeby.etherscan.io/token/0xb9c286126cbf8286f2c9b77b84ab9f33cd5faad4?a=0xe2cdfDAE0144F1AE8396e65c263F1b744771a574

## Installation

```bash
$ npm install
```

## Deploing contract

Create your .env file with data: YOUR_ALCHEMY_API_URL, YOUR_PRIVATE_RINKEBY_ACCOUNT_KEY. And run command below:

```bash
$ npm run deploy
```

## Test

```bash
$ npm test
```

## License

MIT
