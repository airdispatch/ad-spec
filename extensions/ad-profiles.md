Airdispatch Profiles
==================

### Introduction

The Airdispatch Profiles protocol will be responsible for converting Airdispatch Addresses into familiar names, faces, and information.

### Messages

The Airdispatchs Profiles protocol functions by having a publicly available message under the id `profile`.

This message MUST contain the following DataTypes:

- `airdispat.ch/profiles/name` - The full name of the Airdispatch User
- `airdispat.ch/profiles/photo` - A URL of a Photo to represent the User's profile picture it must be over HTTP and publicly accessible