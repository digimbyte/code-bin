**How to use**
Make a post request to:

testnet: `http://seed5t5.neo.org:20332`

mainnet: `https://node.tothemoonuniverse.com`


**getTokens request payload**
```js
{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "invokefunction",
    "params": [
        "0x4fe8c3f1423163148d45960cdb5e141da8e3ab81",//contract hash
        "tokensOf",
        [
            {
                "type": "Hash160",
                "value": "0xb628c23ce5bd8bb1dce62e2b290d8ceb73554657" //Neo 3 address to script hash
            }
        ]
    ]
}
```

**traverse iterator request payload**
```js
{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "traverseiterator",
    "params": [
        "bd819ab9-688e-42e3-883f-6465c67c3887",
        "3781fdc8-f54c-4219-86bf-14a077062f90",
        100 //max quantity results
    ]
}
```

**properties request payload**
```js
{
    "jsonrpc": "2.0",
    "id": 1,
    "method": "invokefunction",
    "params": [
        "0x4fe8c3f1423163148d45960cdb5e141da8e3ab81",//contract hash
        "properties",
        [
            {
                "type": "ByteArray",
                "value": "TUQy" //tokenId of an nft (base64)
            }
        ]
    ]
}
```
