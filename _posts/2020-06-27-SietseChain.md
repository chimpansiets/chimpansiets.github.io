---
layout: post
title: SietseChain
---

My own Blockchain written in Python, capable of mining blocks and making transactions using the Python Flask framework.
I started this project by following a [tutorial](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46) about how to create your own blockchain.
This is obviously not meant to be an amazing functional blockchain (in fact, it is a pretty crappy one), but this project gave me a better understanding 
of how blockchain networks function in detail, simply for research purposes.

## Getting started

### Downloading

`git clone https://github.com/chimpansiets/own_blockchain.git`

or download the ZIP from

(https://github.com/chimpansiets/own_blockchain)

### Running

```
$ python blockchain.py
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

You can use cURL or Postman to interact with this API over a network.

Firstly, try mining a block by making a GET request to `http://localhost:5000/mine`:

![get_request_picture](https://hackernoon.com/photos/JTw2M3rQabaxNg3EFoNIxjmC1ZB3-dk232gk "get_request_picture")

After, create a new transaction by making a POST request to `http://localhost:5000/transactions/new` with a body containing our transaction structure:

![transaction_picture](https://hackernoon.com/photos/JTw2M3rQabaxNg3EFoNIxjmC1ZB3-p31b132c2 "transaction_picture")

If you are not using Postman, then you can make the same request using cURL:

```
$ curl -X POST -H "Content-Type: application/json" -d '{
 "sender": "d4ee26eee15148ee92c6cd394edd974e",
 "recipient": "someone-other-address",
 "amount": 5
}' "http://localhost:5000/transactions/new"
```

## Resources / External Links

* https://hackernoon.com/learn-blockchains-by-building-one-117428612f46
