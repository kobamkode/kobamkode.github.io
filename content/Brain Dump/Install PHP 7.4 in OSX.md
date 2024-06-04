---
date: 2024-05-31
tags:
    - php
---
```sh
brew tap shivammathur/php
brew install php@7.4
brew unlink php@8.3
```
add this into .zshrc file:
```sh
export PATH="/usr/local/opt/php@7.4/bin:$PATH"
export PATH="/usr/local/opt/php@7.4/sbin:$PATH"
```
don't forget to `source ~/.zshrc`.

If you want to rollback into latest version which you have installed before,
just do the vice versa.
