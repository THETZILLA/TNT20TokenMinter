**TNT20TokenMinter**
**Quick tutorial on how to release your own TNT20 token on the Theta Network**


1) Copy the contents of 'contract.sol'
2) Go to https://remix.ethereum.org/ and create a new file in your workspace.
   - Right click on workspace + create new file.
   - Name the file... Remix will automatically set it as .sol extension.
   - Paste the previously copied content of the contract.sol file and save the file (cmd + s / ctrl + s).
   - Go to the compilation tab (should be giving you an error by now)
   - Once there, change the compiler version to 0.7.4 and then click on compile.
   - Once compiled and having no errors, chose the MINTABLETNT20 in the contract dropdown then copy the ABI and bytecode.

   <img width="566" alt="image" src="https://github.com/THETZILLA/TNT20TokenMinter/assets/156357319/a6d60f29-8607-4ff6-9a47-2e7b817a1fb6">

   
4) Create a new wallet on Theta (https://wallet.thetatoken.org/create)
   - Click on "Contracts"
   - Deploy new contract
   - Here you paste the info from Remix. The ABI and the ByteCode from the tnt20 contract.
   - Pick NAME, SYMBOL, DECIMALS, INITIAL SUPPLY and set mintable to true
   - Click on DEPLOY CONTRACT (you must have TFUEL in the wallet balance to pay for the gas fees).
   <img width="1081" alt="image" src="https://github.com/THETZILLA/TNT20TokenMinter/assets/156357319/1b26bae1-4f2a-4257-8128-2d608ad64299">

5) The contract has been created. In this example we created contract address: "0xf1ca2dc3037c8d22a4aa4b508990d0b9acf86548"
6) Now we are going to publish the contract. Open ThetaExplorer (https://explorer.thetatoken.org/) and paste the contract address.
7) Find the contract tab and paste the contents of your contract taken from REMIX (Here is where you can add the contract address to the comments and your website, twitter account, etc). Click on verify and publish
   <img width="1066" alt="image" src="https://github.com/THETZILLA/TNT20TokenMinter/assets/156357319/b85212ef-510d-4820-be9a-faf16038fc50">

**And we are done!**

   If you have done everything correctly this is the way the contract should look:
   <img width="989" alt="image" src="https://github.com/THETZILLA/TNT20TokenMinter/assets/156357319/8826de86-e55f-4cbd-b5f2-020b4e1dc7b3">

