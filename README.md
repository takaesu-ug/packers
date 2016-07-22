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

Todo
-------------

* centos6.7は ipv6 関連を無効にする
  * [vagrant環境下で \[Errno 14\] PYCURL ERROR 6 – “Couldn’t resolve host エラー | blog@human](http://blog.at-human.com/2015/02/08/vagrant%E7%92%B0%E5%A2%83%E4%B8%8B%E3%81%A7-errno-14-pycurl-error-6-couldnt-resolve-host-%E3%82%A8%E3%83%A9%E3%83%BC/)

Thanks
-------------

https://github.com/shiguredo/packer-templates
