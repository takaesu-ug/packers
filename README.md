My Packer Template Example
==============

Builded boxes
------------

https://atlas.hashicorp.com/yusabana

Usage
-------------

### In Local

Build box for vagrant at the local.

```
packer build template_local.json
```

### In Atlas

IMPORTANT: You create TOKEN and set env `export ATLAS_TOKEN='token strings'` before pushing.

Push to build box for vagrant at the atlas.

```
packer push -name USERNAME/ATLASBUILD_NAME template_atlas.json
```

NOTE: Add double-array in post-procesors with using Atlas. Refer below.

* [Missing metadata.json (Packer (push) -> ATLAS (build) -> Vagrant (download)) · Issue #2090 · mitchellh/packer](https://github.com/mitchellh/packer/issues/2090)

Thanks
-------------

https://github.com/shiguredo/packer-templates
