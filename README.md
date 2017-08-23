# cabinet

Exploring a new notebook container format

## Proposal

* Entire "cabinet" is a directory of files and can be read either as a directory (read: git repo) or as a zip file
* Notebook source (markdown and code) is in a markdown file
* Images and other outputs end up in separate "sidecar" files
* (somehow) metadata for outputs gets persisted
* There's a manifest at the top layer to help tie this all together

The reason we're exploring this is for

* git friendliness, while keeping outputs.
* size friendliness, by virtue of having images and other binary data separate

