# ⚡️ tkolleh's Git Commands [![starline](https://starlines.qoo.monster/assets/tkolleh/git-commands)](https://github.com/qoomon/starline)

Git commands for common tasks with interactive fzf-powered interfaces.

## Installation

1. Clone this repository

```zsh
gh repo clone tkolleh/git-commands
```

2. Make all scripts executable

```zsh
chmod +x git-commands/git-*
```

3. Add the directory to your `$PATH` (add to `~/.zshrc` for persistence)

```zsh
export PATH="$HOME/path/to/git-commands:$PATH"
```

4. Set `$FZF_GIT_HOME` to your fzf-git.sh installation

```zsh
export FZF_GIT_HOME="$HOME/path/to/fzf-git.sh"
```

## Dependencies

| Tool | Purpose | Install |
|------|---------|---------|
| [fzf](https://github.com/junegunn/fzf) | Fuzzy finder for interactive selection | `brew install fzf` |
| [fzf-git.sh](https://github.com/junegunn/fzf-git.sh) | Git+fzf integration (required) | Clone and set `$FZF_GIT_HOME` |
| [gum](https://github.com/charmbracelet/gum) | Interactive prompts for commit messages | `brew install gum` |
| [gh](https://cli.github.com/) | GitHub CLI | `brew install gh` |

## Commands

| Command | Description |
|---------|-------------|
| `git aliases` | Interactive alias viewer with fzf |
| `git branches` | Browse and select branches with fzf |
| `git brief` | Enhanced git status with diff stats per file |
| `git comm` | Interactive [conventional commit](https://www.conventionalcommits.org/) message generator |
| `git commits` | Browse commit history with fzf |
| `git files` | Browse tracked files with fzf |
| `git remotes` | Browse remotes with fzf |
| `git stashes` | Browse stashes with fzf |
| `git tags` | Browse tags with fzf |
| `git worktrees` | Browse and switch worktrees with fzf |

Use `-h` or `--help` with any command for detailed usage information.

## Aliases

[common-git-cmd-aliases.conf](common-git-cmd-aliases.conf) contains a collection of useful git aliases.

### Installation

1. Copy the alias file to your local config directory:

```zsh
cp common-git-cmd-aliases.conf ~/.local/share/git/
```

2. Include it in your `~/.gitconfig`:

```ini
[include]
  path = ~/.local/share/git/common-git-cmd-aliases.conf
```

## References

* Inspired by [ttscoff/git-commands](https://github.com/ttscoff/git-commands)
