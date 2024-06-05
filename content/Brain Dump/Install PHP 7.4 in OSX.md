---
date: 2024-05-31
tags:
    - php
---
**Problem**: I need to switch between the old PHP version and the new one to maintain some websites. 
unfortunately, I found that the old PHP version is not included in homebrew, so I need to tap from community repository to get them.
```sh
brew tap shivammathur/php
brew install php@7.4
brew unlink php@8.3
```
add these lines into the .rc file:
```sh
export PATH="/usr/local/opt/php@7.4/bin:$PATH"
export PATH="/usr/local/opt/php@7.4/sbin:$PATH"
```
don't forget to `source` the .rc file or restart the terminal window.

If you want to rollback into the latest installed PHP version,
you could do `brew unlink` and `brew link` the PHP version that you wish to rollback.
Don't forget to change the exported PHP version path in the .rc file. 

If you need to switch between version of composer, maybe [[Brain Dump/Downgrade Composer to v1]] could help.
