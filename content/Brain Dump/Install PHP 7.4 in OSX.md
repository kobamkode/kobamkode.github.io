---
date: 2024-05-31
tags:
    - php
---
**Problem**: I need to switch between old PHP version and the new one to maintain some legacy websites. 
I found that the old version of PHP is not included in homebrew, so I need to tap from community repository to get them.
```sh
brew tap shivammathur/php
brew install php@7.4
brew unlink php@8.3
```
add this into .rc file:
```sh
export PATH="/usr/local/opt/php@7.4/bin:$PATH"
export PATH="/usr/local/opt/php@7.4/sbin:$PATH"
```
don't forget to `source ~/.zshrc`.

If you want to rollback into latest installed version of PHP,
you could `unlink` and `link` the version of php that you wish to rollback 
and don't forget to change the version of the exported PATH in .rc file. 

If you need to switch between version of composer, maybe [[Brain Dump/Downgrade Composer to v1]] could help.
