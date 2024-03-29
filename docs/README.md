<h2 align="center">
  <a href="https://github.com/z-shell/zi">
    <img src="https://github.com/z-shell/zi/raw/main/docs/images/logo.svg" alt="Logo" width="80" height="80" />
  </a>
❮ ZI ❯ Package - NB
</h2>

<h3 align="center">

| **Package source:** | Source Tarball | Git | Node | Gem |
| :-----------------: | :-----: | :-: | :--: | :-: |
|     **Status:**     | :heavy_check_mark: (default) |  -  | :x: | :x: |

</h3>

Provides CLI and local web plain text note‑taking, bookmarking, and archiving with linking,
tagging, filtering, search, Git versioning & syncing, Pandoc conversion, + more, in a single portable script.

The package installed locally into a plugin directory (feature of
the bin-gem-node annex) and provided to the command line through _shims_, i.e.:
automatic forwarder scripts created under `$ZPFX/bin` (which is added to the
`$PATH` by default; shims are also a bin-gem-node annex feature).


### Available `pack''` invocations

```zsh
zi pack for nb
```

### Default Profile

```shell
zi ice as'completion' nocompile sbin'nb' \
  depth'3' atclone'mv -vf etc/nb-completion.zsh _nb'
zi light @xwmx/nb
```

```shell
# Same as above, except using the For syntax
zi for as'completion' nocompile sbin'nb' \
  depth'3' atclone'mv -vf etc/nb-completion.zsh _nb' \
    @xwmx/nb
```

---

> This repository compatible with [ZI](https://github.com/z-shell/zi)

The [xwmx/nb](https://github.com/xwmx/nb/) zsh package that can use the NPM package registry to automatically:

- get the plugin's Git repository OR release-package URL,
- get the list of the recommended ices for the plugin,
  - there can be multiple lists of ices,
  - the ice lists are stored in _profiles_; there's at least one profile, _default_,
  - the ices can be selectively overridden.
