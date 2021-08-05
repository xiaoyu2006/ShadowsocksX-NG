# ShadowsocksX-NG

[Download](https://github.com/ssx-ng/ShadowsocksX-NG/releases/latest)

[![Actions Status](https://github.com/ssx-ng/ShadowsocksX-NG/workflows/CI/badge.svg)](https://github.com/shadowsocks/ShadowsocksX-NG/actions)

Next Generation of [ShadowsocksX](https://github.com/shadowsocks/shadowsocks-iOS)

## Requirements

### Running

macOS 10.12+

### Building

- Xcode 12.5.1+
- CocoaPods 1.10.1+

Run `pod install` then open the Xcode workspace.

## Download

From [here](https://github.com/ssx-ng/ShadowsocksX-NG/releases/)

## Features

- `sslocal` from shadowsocks-rust.
- Support SIP003 plugins. Embed `kcptun`,  `simple-obfs` and `v2ray-plugin`.
- Could update PAC by download GFW List from GitHub.
- Share your server profiles by qrcode or url.
- Import server profile urls from pasteboard.
- Import server profile by scan QRCode on screen.
- Custom rules for PAC.
- Support for [AEAD Ciphers](https://shadowsocks.org/en/spec/AEAD-Ciphers.html)
- HTTP Proxy by [privoxy](http://www.privoxy.org/)

## Difference from original ShadowsocksX

`sslocal` is run as a background service through launchd, not as an in-app process.
So after you quit the app, the `sslocal` might be still running.

Added a manual mode which won't configure the system proxy settings,
so that you could configure your apps to use the SOCKS5 proxy manually.

## Contributing

Contributions must be available on a separately named branch based on the latest version of the main branch `develop`.

ref: [GitFlow](http://nvie.com/posts/a-successful-git-branching-model/)

## License

The project is released under the terms of the GPLv3.

