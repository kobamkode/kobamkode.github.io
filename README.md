# Kobamkode

## Setup
- Install Hugo
```sh
CGO_ENABLED=1 go install -tags extended github.com/gohugoio/hugo@latest
```
- Install [Typo](https://github.com/tomfran/typo/wiki/Setup) Theme
```sh
git submodule add --depth=1 https://github.com/tomfran/typo.git themes/typo
```
- If it says 'themes/type already exists in the index', unstage the themes directory first the readd submodule

```sh
git rm -r themes
```
