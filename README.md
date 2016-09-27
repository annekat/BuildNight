# Notes for September 27th Build Night
_Welcome Innovation Tribe_

## Getting Started Information
Hello World
https://docs.docker.com/engine/tutorials/dockerizing/

Docker Setup
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-getting-started

## Testing and CI/CD

Hound
https://houndci.com/

Circle CI
https://circleci.com/features/

GoCD
https://www.go.cd

### golang
**Starter Program**
https://github.com/Kindafearless/goserver

Go Testing
http://jonathanmh.com/golang-unit-testing-for-absolute-beginners/

Travis CI
https://docs.travis-ci.com/user/languages/go

## Deployment
Setup Command Line
https://devcenter.heroku.com/articles/heroku-command-line

Heroku Go Deployment
https://devcenter.heroku.com/articles/getting-started-with-go#prepare-the-app

Heroku Docker Config
https://devcenter.heroku.com/articles/container-registry-and-runtime

AWS Deployment - ECS
http://docs.aws.amazon.com/AmazonECS/latest/developerguide/docker-basics.html

Simple activities
1. Fork a simple Go app (search github for this)

3. Create a .yaml file


1. Fork the GoServer from kindafearless
2. Add a test file to the go App in Git (*note, it doesn't have to be a real test. You can copy and paste any test, you want it to fail)
3. Update the yaml file with script: ./hello_test (or the name of your test file)
4. Add the forked repo with Travis CI
5. 

For deploying to Heroku
- Follow the instructions https://devcenter.heroku.com/articles/deploying-go
* you need this file to deploy to heroku
Add the repo to Travis CI
