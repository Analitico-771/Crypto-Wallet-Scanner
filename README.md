1. This app gets the balance of a crypto wallet from the blockchain and calculates the current market value.  This was my first app to pull data from the blockchain.  I also used a .env file to protect addresses/api keys/and node points.

This script showcases how to get data from the blockchain while protecting sensitive information

To make this work git clone this repository:
1. npm install web3   https://web3js.readthedocs.io/en/v1.3.4/
2. npm install node-fetch   https://github.com/node-fetch/node-fetch
3. npm install dotenv   https://github.com/motdotla/dotenv
4. code .env and give values to the variables as you see in the .env_example.  Add the .env to your .gitignore file
5. I have node 15 globally installed. You may need to npm i -y or npm init if you have issues with any of the dependencies.  Also try to close your text editor and reopen it.  I work with VS Code with files on Dropbox switching between 2 computers and have no issues.
6. Finally, you need to verify the returned object structure on your API call from wherever you're getting the current price info. Then update/change the reference to symbolData.price on line 29 if needed.

The one I used looks like this:
{ exchange: 'gdax',
  pair: 'linkusd',
  price: 17.19823,
  ask: 17.20994,
  bid: 17.19823 }

* Tech Stack
    * Languages: JS, Solidity
    * Other: Ethereum, JSON, Postman, Web3

* Screenshots Our App
    * ![](/images/app_image.jpg)

* Developer Team
    * Jose Tollinchi
    * https://github.com/AnaIitico