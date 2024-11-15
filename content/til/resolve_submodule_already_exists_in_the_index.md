+++
title = 'Resolve Submodule Already Exists in the Index'
slug = 'resolve-submodule-already-exists-in-the-index'
date = 2024-11-15T18:04:49+07:00
draft = false
tags = ['git']
showTags = true
hideBackToTop = true
+++

Today I learned to resolve an error like "...already exists in the index" when adding a submodule. To resolve, unstage the submodule first using the `git rm -r your_submodule_dir` command and then re-add it.
