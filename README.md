# WiVRn for Debian

Unofficial Debian packages of [WiVRn](https://github.com/WiVRn/WiVRn).

This repository contains only build automation. A GitHub Actions workflow
checks daily for a new upstream WiVRn release, builds a `.deb` for Debian 13
(trixie, amd64) and publishes it on the [Releases](../../releases) page under
the same tag as upstream.

## Installing

Download the `.deb` from [Releases](../../releases) and install it:

```sh
sudo apt install ./wivrn_*_amd64.deb
```

For setup, usage and troubleshooting, see the
[WiVRn repository](https://github.com/WiVRn/WiVRn).

## Issues

Problems with WiVRn itself belong in the
[WiVRn issue tracker](https://github.com/WiVRn/WiVRn/issues). Only report
issues here if they are about the packaging or the build workflow.

## Building

The workflow is in [`.github/workflows/build.yml`](.github/workflows/build.yml).
It runs on a schedule and can also be started by hand from the Actions tab,
optionally with a specific upstream tag.

## License

WiVRn is licensed under GPL-3.0. This project is not affiliated with WiVRn.
