# demo-bonita-chain

This repo contains the materials to show how to integrate Bonita BPM with Chain.

The use case demonstrated in this demo is a car supply chain. 

A recording of the video is available [here](http://www.bonitasoft.com/for-you-to-read/videos/accelerate-blockchain-technology-adoption-bonita-bpm-and-chain-core). 

# Requirements

To run the demo on your machine you will need the following elements:
* [Bonita Studio 7.4.1 minimun](www.bonitasoft.com/downloads-v2)
* [Chain core](https://chain.com)
* [Chain connectors for Bonita](https://github.com/Bonitasoft-Community/bonita-connector-chain)

# Installation

* Start Chain core and connect to Test Network

* Build the project InitChain
```
cd InitChain
mvn package
```

* Run the project InitChain to init the Chain Test Network with the data for the demo
```
mvn exec:java -Dexec.mainClass="org.bonitasoft.chain.InitDemoSupplyChain"
```

* Start Bonita Studio
* Import the process (process/CarSupplyChain-1.0.bos)
* Run the process
