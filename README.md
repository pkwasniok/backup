# backup

Documentation of my backup solution.

## Table of contents

1. [Intro](#intro)
2. [Archivization](#archivization)
3. [Compression](#compression)
4. [Encryption](#encryption)
5. [Storage](#storage)

## Intro

My main goal was to keep the backup process as simple as possible. It is built
only uppon open-source tools, that are available in most package repositories.
Whole backup creation process can be executed in one command.

## Archivization

Archivization is based on `tar` tool.

```sh
tar --create --file [output file] [input dir]
```

## Compression

Compression is based on `zstd` tool.

```sh
zstd --output [output file] [input file]
```

## Encryption

Encryption is based on `age` tool.

```sh
age --encrypt --passphrase --output [output file] [input file]
```

## Storage

Storage solution is not yet determined.

