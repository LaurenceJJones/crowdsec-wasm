## Crowdsec WASM

This repository is an attempt to port some of crowdsec functionality over to WASM. Reasoning behind this is to allow tooling to be created that can use javascript for example

- Create parsers and scenarios via a web UI and get direct feedback on if it works
- Run a log file or line through crowdsec detection engine and get feedback directly on the website (purely client side only)

#### Inital POC

I still don't know if this is even doable, so ATM I am going to use this as a POC. The initial POC will attempt to get an instance of Crowdsec (all available parsers / scenarios) running within a javascript object. Once this function is complete the ability to run an array of log lines similar to `cscli explain`. If this is successfull then I can attempt to create smaller functions attributed to the Crowdsec type.

> What it takes to be a successfull POC?

> The WASM function must be able to parse the hub .index.json and process a log line to inform the user what crowdsec detected similar to the `explain` cscli command
