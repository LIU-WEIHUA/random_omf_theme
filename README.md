# random_omf_theme🐠
randomly install and enable themes from [official packages repository](https://github.com/oh-my-fish/packages-main) of [oh-my-fish/oh-my-fish](https://github.com/oh-my-fish/oh-my-fish)  for [fish shell](https://fishshell.com/)
### Installation & Usage🛫
Install [oh-my-fish/oh-my-fish](https://github.com/oh-my-fish/oh-my-fish#installation) for the fish shell first. And then execute these commands in the fish shell.
```
git clone --depth=1 https://github.com/MilkyMAISHIRANUI/random_omf_theme $OMF_PATH/themes/random_omf_theme
```
To enable random themes, type this.
```
omf theme random_omf_theme
```
If random_omf_theme is enabled already, `omf theme random_omf_theme` does nothing. So it does with other themes. Please use above command instead.
```
omf reload
```
We are not listed in the oh-my-fish packages repository. Therefore you could not use the `omf install random_omf_theme` command.
### Known Issues ⚠️
 `fish_config` command persists the prompt to `~/.config/fish/functions/fish_prompt.fish` . That file takes precedence over Oh My Fish's themes. Therefore command `omf theme <theme_name>` will not work.  `aight`,`boxfish`,`sashimi`,`slavic-cat` and other themes will cause this issue.
To fix it as `omf doctor` suggested, enter this command.
```
rm ~/.config/fish/functions/fish_prompt.fish
```
