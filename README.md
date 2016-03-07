My Packer Template Example
==============

Usage
-------------

### In Local

build box for vagrant at the local.

```
packer build template_local.json
```


### In Atlas

Push to build box for vagrant at the atlas

```
packer push -name USERNAME/ATLASBUILD_NAME template_atlas.json
```

NOTE: You create TOKEN and set env `export ATLAS_TOKEN='token strings'` before pushing.


Thanks
-------------

https://github.com/shiguredo/packer-templates
