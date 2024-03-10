---
title: Store Cheatsheets With Navi
draft: false
date: 2024-03-10
tags:
  - tools
---

## Installation

Cargo is my preference to install navi,
```sh
cargo install navi
```

for OSX,
```sh
brew install navi
```

## Usage

- Type `navi` in terminal

### Add custom cheatsheet into navi

- Create a repository in Github with public access, clone it to local.
- Create cheatsheet file `.cheat` extension, eg: `my.cheat`.
- Follow the syntax to create a cheatsheet, eg:
  ```sh
  % env

  # print all environment variables
  printenv
  ```
  - `%`: beginning of cheatsheet and should contain tags.
  - `#`: description of cheatsheet.
  - more information about syntax is [here](https://github.com/denisidoro/navi/blob/master/docs/cheatsheet_syntax.md#cheatsheet-syntax).
- Push cheatsheet from your local to Github.
- Pull cheatsheet into navi with navi command,
  
  ```sh
  navi repo add <cheatsheet_github_repo>
  ```
- After pull process is completed, type `navi` to display cheatsheets.
  - Type `env` and find a description `print all environment variables`.
  - Press `enter`, the terminal will display a list of environment variables.
- Done.



## Reference

- https://github.com/denisidoro/navi
