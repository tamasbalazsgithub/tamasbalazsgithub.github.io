## GitLab CI

This project's static Pages are built by [GitHub CI][ci], following the steps
defined in [`.github-ci.yml`](.github-ci.yml):

```
image: alpine:latest

pages:
  stage: deploy
  script:
  - echo 'Nothing to do...'
  artifacts:
    paths:
    - public
  only:
  - main
```

The above example expects to put all your HTML files in the `public/` directory.

## Github User or Group Pages

To use this project as your user/group website, you will need one additional
step: just rename your project to `namespace.github.io`, where `namespace` is
your `username` or `groupname`. This can be done by navigating to your
project's **Settings**.
