# fish config

Personal fish shell configuration with bang-bang history expansion, PATH setup, and aliases.

## Features

- `!!` — expand previous command
- `$!` — expand previous command's arguments
- Works with default, vi, and hybrid key bindings
- Adds `~/.local/bin` and `~/.cargo/bin` to PATH
- `rm` aliased to `rm -rfv`

## Install

Copy `config.fish` to `~/.config/fish/config.fish`, then reload:

```sh
source ~/.config/fish/config.fish
```

## Usage

```
$ echo hello
$ !!         # expands to: echo hello
$ sudo !!    # expands to: sudo echo hello
$ $!         # expands to: hello (last argument)
```

## Notes

- `rm` is aliased to `rm -rfv` — **no confirmation prompt, deletes recursively**. Be careful.
