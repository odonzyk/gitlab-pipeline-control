![Build Status](https://gitlab.com/pages/plain-html/badges/master/build.svg)

---


## GitLab Pipeline Control

Provide a short solution with eg. Gitlab Pages for:


    - Generate Run Pipeline form with pre-filled variables  
    - Trigger pipelines over a simple frontend with given variable combinations
    - Usage of API calls in the background
    - Own frontend System to provide individual view´s & controlls


**Get a first preview** https://donzyk.gitlab.io/gitlab-pipeline/   
**or open the screen-capture** https://gitlab.com/donzyk/gitlab-pipeline/-/blob/master/Screen_Capture_-_Gitlab_Control_-_donzyk.gitlab.io.png


The functionality comes from the bottom of the index.html (java script, jquery)!

Search for "//todo" remarks to fill in your token and Project ID it's needed for the API call's




This project's static Pages are built by [GitLab CI][ci], following the steps
defined in [`.gitlab-ci.yml`](.gitlab-ci.yml):

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
  - master
```

## special thanks goes to

    Guido Lange
    https://github.com/gylxan

    and

    Arthur Lerke

    for working on the js and gitlab-ci.yaml solutions.
    It was a great teamwork ;-)
