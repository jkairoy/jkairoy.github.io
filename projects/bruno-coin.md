---
layout: post
title: "Bruno Coin"
description: "Creating a simple, Satoshi client based cryptocurrency"
image_position: center
gradient_colors: ["rgba(216, 88, 65, 1)", "rgba(55, 123, 209, 1)"]
background_color: "#9A25CC"
categories: [GoLang, Blockchain, gRPC, Protocol Buffers, uber-go/atomic, Distributed Consensus]
date: 2021
---
## Background
During the summer of 2021, I worked as a teaching assistant for [CSCI 1951L Blockchains and Cryptocurrencies](http://cs.brown.edu/courses/cs1951l/). As a TA, I took the lead role in developing the first assignment for the class, "Bruno Coin". Bruno Coin is a barebones cryptocurrency based off of the original Bitcoin client. The client was written in GoLang using gRPC for networking between clients.

## Features
* **Node discovery**: discovery in Bruno Coin is done using seed nodes to start a graph, eventually expanding into a full graph where nodes may become connected to many nodes upon requesting a connection from a single node through neighbor propagation.
* **Bootstrapping**: nodes joining the network can bootstrap from other nodes to receive a full record of the chain.
* **Transaction and block validation**: validation of transactions and blocks is done using a simplified version of the Bitcoin verification specifications. 

Like all functional cryptocurrencies, Bruno Coin can handle forked chains and malicious nodes. 

## Autograder
I created an autograder to score students on their submissions using a combination of python and bash. I am happy to report that the average score for the assignment was above the "A" threshold!
