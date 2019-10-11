# Node.js bumble api

Unofficial API for interacting with the dating app Bumble

## Getting Started

```
npm install bumbleapi
```

## How to use 

```
var BumAPI = require('bumbleapi')('Your telephone','Your password');
```
To initalize you need to run
```
BumAPI.startup().then((res) => {console.log(res);})
```

Run BumAPI.startup() to initialize the session. 

Then you can run BumAPI.getEncounters().

In the BumAPI.getEncounters() response you can find the encounters info and ids

To submit a vote no BumAPI.voteNoForEncounter(id) where the id can be found in the response of BumAPI.getEncounters().

To submit a vote yes BumAPI.voteYestForEncounter(id) where the id can be found in the response of BumAPI.getEncounters().

# 3 functions are curenctly available
```
BumAPI.getEncounters().then(data => {})
```
```
BumAPI.voteNoForEncounter(id).then(data => {})
```
```
BumAPI.voteYestForEncounter(id).then(data => {})
```

## Contributing

Please email konakia@gmail.com for more info.

## License

This project is licensed under the ISC License
