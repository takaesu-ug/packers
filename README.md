My Packer Template Example
==============

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


Thanks
-------------

https://github.com/shiguredo/packer-templates
