yarn add web3
yarn start

//web3.eth.sendTransaction
web3.eth.getAccounts()

let ac1 = '0x7Df3a7536F086F4B3AFEB4692f3ec0a164511e8C'
web3.eth.sendTransaction({from:ac1, to:'0x4762e30D015f6D232D1A92A570E548Df460e27E2',value:10000000000000000000}) => 10eth 
--------------------------------------


https://www.textfixer.com/tools/remove-line-breaks.php

https://web3js.readthedocs.io/en/v1.2.3/web3-eth-contract.html#id52



truffle migrate --reset
truffle console

Lottery.deployed().then(function(instance){lt=instance})
lt
web3.eth.getAccounts()
let bettor = '0x7Df3a7536F086F4B3AFEB4692f3ec0a164511e8C'
lt.betAndDistribute
lt.betAndDistribute('0xab', {from:bettor, value:5000000000000000, gas:300000})

lt.getBetInfo(1)


-------------------------------------

Dapp 데이터 관리

- Read
    - smart contract를 직접 call, batch read call
    - event log를 읽는 방법
        - http(polling)
        - websocket
1. init과 동시에 past event 들을 가져온다.
2. ws으로 geth 또는 infura와 연결한다.
3. ws으로 원하는 이벤트를 subscribe 한다.
    a. ws을 사용할 수 없다면 롱 폴링을 이용한다(롱 폴링은 3초에 한번씩 일어낫니 물어본다)
4. 돈이 크게 걸려있는 서비스 -> 블락 컨펌 확인


-----------------------------------------

yarn add bootstrap -> 부트스트랩 사용


--------------------------------------

Dapp 서비스

1. 비즈니스 로직(로터리)
2. 스마트 컨트랙트
    a. 블록체인에 배포(ganache-cli)
3. Dapp - front
    a. react.js




