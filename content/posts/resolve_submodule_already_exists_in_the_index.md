+++
title = 'Resolve Git Submodule Already Exists in the Index'
slug = 'resolve-git-submodule-already-exists-in-the-index'
date = 2024-11-15T18:04:49+07:00
draft = false
tags = ['git']
showTags = true
hideBackToTop = true
+++

Today I learned to resolve an error like "... already exists in the index" when re-adding Hugo's theme submodule. To resolve this error, first unstage the git submodule
```sh
git rm -r --cache <your_submodule_dir>
```
then re-adding Hugo's theme submodule to it's directory
```sh
git submodule add --depth=1 <your_theme_git_url> themes/<your_theme_name>
```
