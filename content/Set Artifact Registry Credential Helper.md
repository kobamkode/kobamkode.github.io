---
title: Set Artifact Registry Credential Helper
draft: false
tags:
  - braindump
  - gcp
  - docker
  - deployment
---
Do authentication before pushing image into Artifact Registry
```
gcloud auth configure-docker asia-southeast2-docker.pkg.dev
```

change `asia-southeast2` to your region.

Reference: https://cloud.google.com/artifact-registry/docs/docker/pushing-and-pulling#cred-helper
