# nvtop (Unraid plugin)

GPU/CPU monitoring TUI based on [Syllo/nvtop](https://github.com/Syllo/nvtop).

## Usage
The plugin puts the `nvtop` command on `PATH`. nvtop is a terminal UI, so run it
from a terminal:

- SSH: `ssh user@server` then `nvtop`
- Web GUI: Settings → Terminal, then `nvtop`

## Files
- Binary:        `/usr/local/emhttp/plugins/nvtop/bin/nvtop`
- Runtime libs:  `/usr/local/emhttp/plugins/nvtop/usr/lib/`
- Runner:        `/usr/local/emhttp/plugins/nvtop/scripts/nvtop-runner`
- PATH symlink:  `/usr/local/bin/nvtop`
- Web page:      Tools → nvtop

## Notes
- The nvtop binary and its ncurses libs are **bundled in the .txz** — no network
  needed at install or boot.
- To update nvtop, install a newer plugin version (bumps the bundled binary).
