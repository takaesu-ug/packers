My Packer Template Example
==============

Usage
-------------

### In local environments

build box for vagrant on the local environment.

```
packer build template_local.json
```


### In Atlas environments

Push to build box file for vagrant on the atlas

```
packer push -name USERNAME/ATLASBUILD_NAME template_atlas.json
```

NOTE: You create TOKEN and set env `export ATLAS_TOKEN='token strings'` before pushing.


Thanks
-------------

https://github.com/shiguredo/packer-templates
