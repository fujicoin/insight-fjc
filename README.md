# Fujicoin Insight UI

A Fujicoin blockchain explorer web application service for [Bitcore Node](https://github.com/bitpay/bitcore-node) using the [Insight API](https://github.com/bitpay/insight-api).

## Getting Started

Dependency: node v4.4.0

```
cd ~/
git clone https://github.com/fujicoin/insight-fjc.git
mv insight-fjc/fujicoin-bitcore-v0.13.2.tar.gz .
tar -zxvf fujicoin-bitcore-v0.13.2.tar.gz
mkdir .fujicoin
mv insight-fjc/fujicoin.conf .fujicoin
# Edit .fujicoin/fujicoin.conf  --- Change username, password
./fujicoin-bitcore/fujicoind &  --- Wait for synchronize to fujicoin network
cd insight-fjc
# Edit ./bitcore-node.json      --- Change datadir, exec, rpcuser, rpcpassword
node_modules/bitcore-node/bin/bitcore-node start
```

Open a web browser to `http://localhost:3001/`
API URL is `http://localhost:3001/api/`

## License
(The MIT License)

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
