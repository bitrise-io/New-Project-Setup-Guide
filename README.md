# New-Project-Setup-Guide

Template / Guide for new projects, from the very first steps to continuous deployment into production.

First, create a Git repository for the new project, then copy-paste the **TODO** section from this Readme to the new project's Readme. Then go through the **TODO** of course ;)

## TODO

- [ ] Setup the base code (generate the template project, e.g. create a new Xcode project or `rails new`)
  - [ ] commit & push
- [ ] Write tests & base functionality, BDD/TDD preferred
- [ ] Setup continuous integration (testing) on [bitrise.io](https://www.bitrise.io)
- [ ] Add linter tools
  - go:
    - [ ] `go test`
    - [ ] `go vet`
    - [ ] [errcheck](github.com/kisielk/errcheck)
    - [ ] [golint](github.com/golang/lint/golint)
    - [ ] __WEB__ [safesql](github.com/stripe/safesql)
  - ruby:
    - [ ] [rubocop](https://github.com/bbatsov/rubocop)
    - [ ] __WEB__ [brakeman](https://github.com/presidentbeef/brakeman)

- [ ] Prepare a staging and a prod env
  - Heroku:
    - [ ] Staging app
    - [ ] Prod app
    - [ ] Heroku pipeline to connect the two
    - [ ] Add this to the readme: How to create a new Heroku app & deploy the project to it
- [ ] Setup continuous deployment for the project - just add it to the existing [bitrise.io](https://www.bitrise.io) config
- [ ] Iterate on the project (and on the automation), test the automatic deployment

Web projects: 

- [ ] Add a log monitoring to the project
  - logentries
