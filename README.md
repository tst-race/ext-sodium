# libsodium for RACE

This repo provides scripts to custom-build the
[libsodium library](https://github.com/jedisct1/libsodium) for RACE.

## License

The libsodium library is licensed under the ISC license.

Only the build scripts in this repo are licensed under Apache 2.0.

## Dependencies

libsodium has no dependencies on any custom-built libraries.

## How To Build

The [ext-builder](https://github.com/tst-race/ext-builder) image is used to
build libsodium.

```
git clone https://github.com/tst-race/ext-builder.git
git clone https://github.com/tst-race/ext-sodium.git
./ext-builder/build.py \
    --target linux-x86_64 \
    ./ext-sodium
```

## Platforms

libsodium is built for the following platforms:

* `android-x86_64`
* `android-arm64-v8a`

It is also used on Linux but can be installed via `apt`.

## How It Is Used

libsodium is used by the <TO-BE-NAMED> plugin.
