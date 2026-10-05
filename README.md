<!-- tyhp-readme:start -->
# tyhpdef/openspout-openspout

Tyhp type definitions for `openspout/openspout` `5.11.3`.

```bash
composer require --dev tyhpdef/openspout-openspout:5.11.3
```

This is a metapackage. Composer also installs `tyhpdef/openspout-openspout-impl` (type files).
Require **this** name, not `tyhpdef/openspout-openspout-impl`.

See https://tyhplang.com.

## Maintain `openspout/openspout`? Ship the types yourself

If you are a Packagist maintainer of `openspout/openspout`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/openspout-openspout-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `openspout/openspout` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/openspout-openspout": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `openspout/openspout` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `openspout/openspout` with a real constraint,
   `"replace": { "tyhpdef/openspout-openspout": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `openspout/openspout` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/openspout-openspout` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
