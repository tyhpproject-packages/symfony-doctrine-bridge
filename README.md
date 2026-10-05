<!-- tyhp-readme:start -->
# tyhpdef/symfony-doctrine-bridge

Tyhp type definitions for `symfony/doctrine-bridge` `7.4.17`.

```bash
composer require --dev tyhpdef/symfony-doctrine-bridge:7.4.17
```

This is a metapackage. Composer also installs `tyhpdef/symfony-doctrine-bridge-impl` (type files).
Require **this** name, not `tyhpdef/symfony-doctrine-bridge-impl`.

See https://tyhplang.com.

## Maintain `symfony/doctrine-bridge`? Ship the types yourself

If you are a Packagist maintainer of `symfony/doctrine-bridge`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-doctrine-bridge-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/doctrine-bridge` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-doctrine-bridge": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/doctrine-bridge` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/doctrine-bridge` with a real constraint,
   `"replace": { "tyhpdef/symfony-doctrine-bridge": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/doctrine-bridge` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-doctrine-bridge` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
