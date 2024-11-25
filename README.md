# torrent-preview.yazi

[Yazi](https://github.com/sxyazi/yazi) plugin to preview `application/x-bittorrent` files

![show case](https://github.com/kirasok/torrent-preview.yazi/assets/75790517/6f215e6d-bb19-46f4-b606-9241594028ff)

## Requirements

- [yazi >= 0.4](https://github.com/sxyazi/yazi)
- [transmission-cli](https://github.com/transmission/transmission)

## Installation

### Linux/MacOS

```sh
ya pack -a boydaihungst/torrent-preview
```

## Usage

Add this to your `yazi.toml`:

```toml
[[plugin.prepend_previewers]]
mime = "application/bittorrent"
run = "torrent-preview"
```
