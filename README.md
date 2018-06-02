# web3-tutorial
web3j a Java and Android library for integrating Smart Contracts into Ethereum network clients/nodes.  
  
Allowing you to access the Ethereum blockchain, without having to write your own integration code everytime your contracts want to comunicate with the Ethereum platform.  
[Java and Blockchain overview video ](https://youtu.be/ea3miXs_P6Y)  
further information:  
* [Project home](http://web3j.io)
* [Mining ](https://docs.web3j.io/transactions.html#obtaining-ether)  
* [useful links](https://docs.web3j.io/links.html)  
* [Chat](https://gitter.im/web3j/web3j)  
* [Conorsvensson.com](http://conorsvensson.com/)
![Web 3 ](https://github.com/charlesfinney/web3-tutorial/blob/master/web3j_network.png)  
   
the way you talk to an ethereum node or client is with a library called web3 over a JSON-RPC or Remote Procedure Call  similar to an API or Application programing interface but instead of a connection to one server the RPC conectes with all nodes  
## Step 1
sign up wih [infura.io](https://infura.io/signup)  
  ![infura](https://github.com/charlesfinney/web3-tutorial/blob/master/infura.png)  
    
    
## Step 2 
download node.js  
  
  ![node.js](https://github.com/charlesfinney/web3-tutorial/blob/master/nodejs.png)
  
## step 3 
setup directory `mkdir web3-tutorial` and set up corresponding git repository 
## step 4 
Next you need to install  web3.js into your project, using the following methods:
  
[web3.js Getting Started](https://web3js.readthedocs.io/en/1.0/getting-started.html)
  
npm: `npm install web3`  
  
If npm install process finds vulneralbilities   
  
  run `npm audit fix` to fix them,
  
After that you need to create a web3 instance and set a provider. Ethereum supported Browsers like Mist or MetaMask will have a `ethereumProvider` or `web3.currentProvider` available. For web3.js, check `Web3.givenProvider`. If this property is `null` you should connect to a remote/local node.
  
> // in node.js use: var Web3 = require('web3');
> 
> var web3 = new Web3(Web3.givenProvider || "ws://localhost:8546");
That’s it! now you can use the `web3` object.  
  
  
