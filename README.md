aws-vault.plugin.zsh

Zsh integration and completions for aws-vault.

## Installation

### Using [zplug](https://github.com/zplug/zplug)
Load aws-vault.plugin.zsh as a plugin in your `.zshrc`

```shell
zplug "alanjjenkins/aws-vault.plugin.zsh", defer:2

```
### Using [zgen](https://github.com/tarjoilija/zgen)

Include the load command in your `.zshrc`

```shell
zgen load alanjjenkins/aws-vault.plugin.zsh
zgen save
```

### Using [Antigen](https://github.com/zsh-users/antigen)

Bundle alanjjenkins/aws-vault.plugin.zsh in your `.zshrc`

```shell
antigen bundle alanjjenkins/aws-vault.plugin.zsh
antigen apply
```

### As an [Oh My Zsh](https://github.com/robbyrussell/oh-my-zsh) custom plugin

Clone aws-vault.plugin.zsh into your custom plugins repo

```shell
git clone https://github.com/alanjjenkins/aws-vault.plugin.zsh $HOME/.oh-my-zsh/custom/plugins/aws-vault
```
Then load as a plugin in your `.zshrc`

```shell
plugins+=(aws-vault)
```

## Caveats

As this plugin loads aws-vault's bash completions adopted for zsh using `bashcompinit` function, make sure that there are no `compinit` calls after the point where it sourced.
