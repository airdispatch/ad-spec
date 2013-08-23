Airdispatch Profiles
==================

### Introduction

The Airdispatch Profiles protocol will be responsible for converting Airdispatch Addresses into familiar names, faces, and information.

### Messages

The Airdispatchs Profiles protocol functions by having a publicly available message under the id `airdispatch_address::profile`.

For example, if one was attempting to get the profile from address `a596aa4e707037a033b638e7b57fb077a1f98cbe7864d6b4`, they would query for the message id `a596aa4e707037a033b638e7b57fb077a1f98cbe7864d6b4::profile`. Legacy and direct addressing is not allowed here.

This message MUST contain the following DataTypes:

- `airdispat.ch/profiles/name` - The full name of the Airdispatch User
- `airdispat.ch/profiles/photo` - A URL of a Photo to represent the User's profile picture it must be over HTTP and publicly accessible