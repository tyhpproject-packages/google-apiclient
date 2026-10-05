<!-- tyhp-readme:start -->
# tyhpdef/google-apiclient

Tyhp type definitions for `google/apiclient` `2.19.4`.

```bash
composer require --dev tyhpdef/google-apiclient:2.19.4
```

This is a metapackage. Composer also installs `tyhpdef/google-apiclient-impl` (type files).
Require **this** name, not `tyhpdef/google-apiclient-impl`.

See https://tyhplang.com.

## Maintain `google/apiclient`? Ship the types yourself

If you are a Packagist maintainer of `google/apiclient`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/google-apiclient-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `google/apiclient` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/google-apiclient": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `google/apiclient` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `google/apiclient` with a real constraint,
   `"replace": { "tyhpdef/google-apiclient": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `google/apiclient` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/google-apiclient` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
