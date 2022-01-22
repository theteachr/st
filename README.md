# Simple Terminal: The Fork

**st** is a simple terminal emulator for X which sucks less.\

Cloned from

```
git://git.suckless.org/st
```

## Build, Install, Run

### Requirements

- Xlib header files

### Installation

Edit config.mk to match your local setup. This fork installs into the following
namespace.

```
$HOME/.local
```

Configuration can be changed by editing `config.h`.

Use the following command to build the terminal.

```sh
make clean install
```

If you did not install with `make clean install`, you must compile
the st terminfo entry (`st-256color`) with the following command:

```sh
tic -sx st.info
```

See the man page for additional details.

Move the generated executable (`st`) to a directory in path (`/usr/local/bin`,
`~/.local/bin`, ...).

##### Credits

Based on Aurélien APTEL <aurelien.aptel@gmail.com> bt source code.
