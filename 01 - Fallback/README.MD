There are two requisites to become the owner of the challenge's contract due to the code "require(msg.value < 0.001 ether);" that's in the contribute function and the code "require(msg.value > 0 && contributions[msg.sender] > 0);" that's in receive() which is the fallback method: to send a contribution greater than 0 and lower than 0.001 ether and to send a transaction greater than 0. I did as follows:

- I sent a contribution greater than 0 with await contract.contribute.sendTransaction({value: 90000000000});. The code is in wei units by default, and it's equivalent to 0.0009 ether.

- I sent a transaction greater than 0.

- I called the withdraw function of the challenge's contract to bring the contract's balance to 0.

![This is an image](https://i.postimg.cc/QM09mHbZ/Ethernaut-1.png)

![This is an image](https://i.postimg.cc/1tXgjsCn/Ethernaut-2.png)

![This is an image](https://i.postimg.cc/26tqpMMH/Ethernaut-3.png)

![This is an image](https://i.postimg.cc/d3ThJnKJ/Ethernaut-4.png)
