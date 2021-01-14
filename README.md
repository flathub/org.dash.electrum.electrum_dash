# org.dash.electrum.electrum_dash

Flatpak build of [Dash Electrum](https://github.com/akhavr/electrum-dash).

## Building

The `python3-requirements*` files are built
using
[these](https://github.com/akhavr/electrum-dash/tree/master/contrib/deterministic-build)
deterministic requirements files,
and `flatpak-pip-generator` from
[flatpak-builder-tools](https://github.com/flatpak/flatpak-builder-tools/), with
a few modifications.


## User data

Wallets are located at `~/.var/app/org.dash.electrum.electrum_dash/.electrum-dash`,
to use `~/.electrum-dash` instead, give the app filesystem permissions

``` sh
flatpak override --filesystem=home org.dash.electrum.electrum_dash
```
