# Alacritty

## Installation

### Imports

Clone the repository, or download the theme of your choice:

```sh
# We use Alacritty's default Linux config directory as our storage location here.
mkdir -p ~/.config/alacritty/themes
git clone https://github.com/alacritty/alacritty-theme ~/.config/alacritty/themes
```

Add an import to your `alacritty.yml` (Replace `{theme}` with your desired
colorscheme):

```yaml
import:
 - ~/.config/alacritty/themes/themes/{theme}.yaml
```

### Config

Replace default config to [custom](../.config/alacritty/alacritty.yml)

[see more](https://github.com/alacritty/alacritty-theme/blob/master/README.md)
