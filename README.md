# Arrase Tmux Theme

A tmux theme forked from catppuccin-tmux.

## Requirements

- tmux 3.0+
- [TPM](https://github.com/tmux-plugins/tpm) (optional)

## Installation

### With TPM

```bash
set -g @plugin 'your-repo/arrase-tmux'
```

### Manual

Add this to your `~/.tmux.conf`:

```bash
source-file /path/to/arrase.tmux
```

## Configuration

### Flavors

This theme supports different Catppuccin flavors:

```bash
set -g @flavour "mocha"  # default: mocha, frappe, macchiato, latte
```

### Window Options

```bash
set -g @window_left_separator "█"
set -g @window_right_separator "█"
set -g @window_middle_separator "█ "
set -g @window_number_position "left"  # or "right"
set -g @window_default_fill "number"   # number, all, none
set -g @window_current_fill "number"   # number, all, none
```

### Status Options

```bash
set -g @status_left_separator ""
set -g @status_right_separator "█"
set -g @status_fill "icon"  # icon, all
set -g @status_connect_separator "yes"
set -g @status_right_separator_inverse "no"

# Modules
set -g @status_modules_right "application session"
set -g @status_modules_left ""
```

Available modules:
- application
- session
- user
- host
- date_time
- directory
- battery
- meetings

## License

MIT
