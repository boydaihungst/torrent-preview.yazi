# torrent-preview.yazi (Deprecated)

> [!NOTE]
> Use [piper.yazi](https://github.com/yazi-rs/plugins/tree/main/piper.yazi#examples) instead: `piper -- transmission-show "$1" --no-header`.
> 
> If you want to highlight tracker urls, install glow and use:
> `piper -- transmission-show "$1" --no-header | CLICOLOR_FORCE=1 glow -w=$w -s=dark -`

[Yazi](https://github.com/sxyazi/yazi) plugin to preview `application/x-bittorrent` files

![show case](https://github.com/kirasok/torrent-preview.yazi/assets/75790517/6f215e6d-bb19-46f4-b606-9241594028ff)

## Requirements

- [yazi >= v25.5.31](https://github.com/sxyazi/yazi)
- [transmission-cli](https://github.com/transmission/transmission)

## Installation

### Linux/MacOS

```sh
ya pkg add boydaihungst/torrent-preview
# or
ya pack -a boydaihungst/torrent-preview
```

## Usage

Add this to your `yazi.toml`:

```toml
[[plugin.prepend_previewers]]
mime = "application/bittorrent"
run = "torrent-preview"
```
