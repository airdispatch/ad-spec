Airdispatch Notes
==================

### Introduction

The Airdispatch Notes protocol is responsible for the formatting of public or private notes in the Airdispatch system.

### Messages

Airdispatch Notes specifies a specific set of DataTypes that declare a public Note.

- `airdispat.ch/notes/title` - The Title of the Note
- `airdispat.ch/notes/content` - The Content of the Note SHOULD be in Markdown format
- `airdispat.ch/notes/category` - The Category of the Note

#### Detecting an Airdispatch Note

A message is considered to be an Airdispatch Note if and only if it contains a Note Title and a Note Content. The Notes Category field is OPTIONAL.