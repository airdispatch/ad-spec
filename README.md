The Airdispatch Protocol
============

This repository will contain the specifications for the Airdispatch protocol.

### Introduction

Airdispatch is a new protocol that seeks to make it easier to provide federated communications platforms. Currently, new services spring up everyday that provide immense functionality to the user with the caveat of being centralized. Airdispatch aims to make more and more products into interoperable services.

The protocol is able to abstract away the problems of addressing, security, and delivery of messages so that developers can focus on the bigger issues. This spec will run through the expected usage of each of the components and how they should interact.

### Table of Contents

  1. Summary of Terms
  2. Message Structure
  3. Message Signatures
  4. Messsage Types
      4.1 Tracker Messages
	  4.2 Server Messages
	  4.3 Client Messages
  5. Server Protocol
  6. Tracker Protocol
  7. Mail Data Format
  8. Race Conditions

### Summary of Terms

  - **Tracker**: Any object in the network graph that responds to tracker messages (Query and Registration) and keeps a database that maps airdispatch addresses to network locations (any resolvable address, IP or URL)
  - **Server**: (Also referred to as the 'mailserver') The location in the network that stores outgoing messages and receives incoming alerts for a specific user. A user may only have one mailserver associated with their address at a time.
  - **Client**: Software that interacts with the user to coordinate the sending and receiving of mail. This software must interact with the server (which actually sends and receives the mail).
