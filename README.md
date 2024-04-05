## Description

```sh
# a unformatted part is reported
$ nix develop --command yamlfmt --lint example.yaml
$ nix develop --command yamlfmt example.yaml

# no unformatted parts are reported
$ nix develop --command yamlfmt --lint example.yaml
$ nix develop --command yamlfmt example.yaml

# `1 files changed` message is reported
$ nix develop --command treefmt --no-cache

# `1 files changed` message is reported again
$ nix develop --command treefmt --no-cache
```
