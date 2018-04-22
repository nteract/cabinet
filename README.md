# cabinet

Exploring a new notebook container format

## Proposal

* Entire "cabinet" is a directory of files and can be read either as a directory (read: git repo) or as a zip file
* Notebook source (markdown and code) is in a markdown file
  * Question: Is it sufficient to denote references to outputs within markdown?
* Images and other outputs end up in separate "sidecar" files
* (somehow) metadata for outputs gets persisted
* There's a manifest at the top layer to help tie this all together

The reason we're exploring this is for

* git friendliness, while keeping outputs.
* size friendliness, by virtue of having images and other binary data separate

## Similar ideas elsewhere

A lot of standard file formats use a compressed directory with a manifest file as their organizing principle.

1. Java [JAR](https://en.wikipedia.org/wiki/JAR_(file_format)) and [WAR](https://en.wikipedia.org/wiki/WAR_(file_format)) formats
2. Open Container Initiative's [Container Image specification](https://github.com/opencontainers/image-spec)
3. [Open Document Format](https://en.wikipedia.org/wiki/OpenDocument)
