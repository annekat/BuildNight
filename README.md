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

## Simplest Activity

1. Fork the GoServer from kindafearless
2. Add a test file to the go App in Git (let's use a hello world test and make it fail)
- name the file "testing"
               package main

              import "testing"

              func TestStubForTesting(t *testing.T){
                expected := "of the burger king"
                actual := StubForTesting()
                if actual != expected {
                  t.Errorf("Test failed, expected: '%s', got:  '%s'", expected, actual)
                }
              }
4. Add the forked repo with Travis CI
5. Copy the token from your account and add it to your github rep *or we found that this happens automatically?
6. In github, select Test 
7. Go back to Travis - you should see the test has failed
8. Add a hello world command to the Git Hub repo so the test will pass
  in goserver.go, add the following command to the very end 
    func StubForTesting() string {
    return "of the burger king"

For deploying to Heroku
- Follow the instructions https://devcenter.heroku.com/articles/deploying-go
* you need this file to deploy to heroku
Add the repo to Travis CI
