There are two requisites to become the owner of the challenge's contract due to the code "require(msg.value > 0 && contributions[msg.sender] > 0);" that's in the fallback method of the challenge's contract: to send a contribution greater than 0 and to send a transaction greater than 0. Here I sent a contribution greater than 0: 

![This is an image](https://i.postimg.cc/QM09mHbZ/Ethernaut-1.png)

Here I sent a transaction greater than 0:

![This is an image](https://i.postimg.cc/1tXgjsCn/Ethernaut-2.png)

And here I called the withdraw function of the challenge's contract to bring the contract's balance to 0:

![This is an image](https://i.postimg.cc/26tqpMMH/Ethernaut-3.png)

![This is an image](https://i.postimg.cc/d3ThJnKJ/Ethernaut-4.png)
