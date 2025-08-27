# ⚡️ tkolleh's Git Commands [![starline](https://starlines.qoo.monster/assets/tkolleh/git-commands)](https://github.com/qoomon/starline)

Git commands for common tasks.

## Installation

1. Download/Clone this repo

```zsh
gh repo clone tkolleh/git-commands
```
2. Make sure all scripts are executable 

```zsh
chmod +x git-commands/git-*
```
3. Add the directory to your $PATH

```zsh
eval "$(realpath git-commands | xargs -I {} echo 'export PATH="{}:$PATH"')"
```

## Dependencies

Some scripts require external tools

* [gum](https://github.com/charmbracelet/gum)
* [fzf](https://github.com/junegunn/fzf)
* [gh](https://cli.github.com/)

## Commands

- `git comm` - write [conventional commit messages](https://www.conventionalcommits.org/en/v1.0.0/#summary) using [Angular conventions](https://github.com/angular/angular/blob/22b96b9/CONTRIBUTING.md#type)
- `git st` - A git status command with [numbered file shortcuts](https://github.com/mroth/scmpuff)

## Aliases

[common-git-cmd-aliases.conf](common-git-cmd-aliases.conf) contains a collection of useful aliases.

### Installation

Save `useful-git-aliases.conf` somewhere on your system. E.g.:

```
  ~/.local/share/git/common-git-cmd-aliases.conf
```

Edit ~/.gitconfig to include this file:

```
  vim ~/.gitconfig
```

Include the path to the alias file:

```
  [include]
  path = ~/.local/share/git/common-git-cmd-aliases.conf
```
## References

* Heavily inspired by [ttscoff/git-commands](https://github.com/ttscoff/git-commands)

## License

This repo is licensed under the MIT License.

See <https://opensource.org/licenses/MIT> for details.
