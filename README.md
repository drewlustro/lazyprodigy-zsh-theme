# LazyProdigy Theme for ZSH
A theme meant for [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/) terminals with a dark background that comes in two flavors, one for local boxes and another to install on servers / remote machines so that you can easily make the distinction with many terminal windows open.
![lazyprodigy.zsh-theme](http://pool.drewlustro.com/img/github/lazyprodigy-ss.png "lazyprodigy.zsh-theme")
---
## Installation

**Note:** The `$ZSH` environment variable must be set, most typically it is set to `~/.oh-my-zsh`. If it is not set, you probably have a broken installation of [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh/).

#### 1. Download Theme

##### via `curl`

```zsh
curl -L https://github.com/drewlustro/lazyprodigy-zsh-theme/raw/master/lazyprodigy.zsh-theme > "$ZSH/themes/lazyprodigy.zsh-theme"
curl -L https://github.com/drewlustro/lazyprodigy-zsh-theme/raw/master/lazyprodigy-server.zsh-theme > "$ZSH/themes/lazyprodigy-server.zsh-theme"
```

##### via `wget`

```zsh
wget --no-check-certificate https://github.com/drewlustro/lazyprodigy-zsh-theme/raw/master/lazyprodigy.zsh-theme -O "$ZSH/themes/lazyprodigy.zsh-theme"
wget --no-check-certificate https://github.com/drewlustro/lazyprodigy-zsh-theme/raw/master/lazyprodigy-server.zsh-theme -O "$ZSH/themes/lazyprodigy-server.zsh-theme"
```

#### 2. Config ZSH To Use LazyProdigy

Edit `~/.zshrc`
```zsh
ZSH_THEME="lazyprodigy"
# or
ZSH_THEME="lazyprodigy-server"
```

#### 3. Customize Machine Name (optional)

LazyProdigy will first check for the presence of `~/.box-name` for the machine name. Otherwise, it will use the result of system command `hostname -s`

---
## Screenshots

`lazyprodigy.zsh-theme`

**Prompt Format:** # USER MACHINE DIRECTORY ♨ git:BRANCH STATE [TIME] \n $ 
![lazyprodigy.zsh-theme](http://pool.drewlustro.com/img/github/lazyprodigy-ss.png "lazyprodigy.zsh-theme")


`lazyprodigy-server.zsh-theme`

**Prompt Format:** ☎ USER ☁ MACHINE ☁ DIRECTORY ♨ git:BRANCH STATE [TIME] \n $ 
![lazyprodigy-server.zsh-theme](http://pool.drewlustro.com/img/github/lazyprodigy-server-ss.png "lazyprodigy-server.zsh-theme")

