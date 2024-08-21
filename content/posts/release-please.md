+++
title = 'Release Please'
date = 2024-08-21T17:44:50+07:00
draft = true
+++

https://github.com/googleapis/release-please/blob/main/docs/cli.md

- Install release-please globally.
    ```
    npm i release-please -g
    ```

- Generate release-please files, it will open pull request againsts the target branch. 
    ```
    release-please bootstrap \
    --token=$GITHUB_TOKEN \
    --repo-url=<owner>/<repo> \
    --release-type=<release-type>
    ```

- Do merge request on Github and pull the merged request


