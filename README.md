![AyeAye](https://github.com/shippableSamples/node-build-push-docker-ecr/blob/master/public/resources/images/captain.png)

# Docker Build, Push to Amazon EC/2 Container Registry and Continuous Integration for a Node JS application
[![Run Status](https://api.shippable.com/projects/588657ed3b7d560f0092e20e/badge?branch=master)](https://app.shippable.com/projects/588657ed3b7d560f0092e20e)
[![Coverage Badge](https://api.shippable.com/projects/588657ed3b7d560f0092e20e/coverageBadge?branch=master)](https://app.shippable.com/projects/588657ed3b7d560f0092e20e)

A simple Node JS application with unit tests and coverage reports using mocha 
and istanbul. Thie repo demonstrates the following features:
  * Set up serverless CI, i.e. on Shippable-provided infrastructure
  * Perform CI tests
  * Perform docker build and push image to Amazon EC/2 Container Registry (ECR)

## Run CI for this repo on Shippable
* Fork this repo into your local repo
* Login into the [Continuous Integration Service](wwww.shippable.com) 
* Create an [integration](http://docs.shippable.com/integrations/imageRegistries/ecr/) on shippable to your docker hub
* All CI configuration is in `shippable.yml`
* Follow these [CI Setup Instructions](http://docs.shippable.com/ci/runFirstBuild/) if you have never used Shippable CI Service
* Update the integrationName in the integration.hub section if you used something other than `avi-beta-gcr`
* Change the DOCKER_REPO and AWS_ECR_URL to point to your repo and registry
* You should be able to run a manual build or webhook build on commit

## CI Reports on Shippable

### CI Integration View
![CI Integration View](https://github.com/shippableSamples/node-build-push-docker-ecr/blob/master/public/resources/images/integration.jpg)

### CI Console Output
![CI Console Output](https://github.com/shippableSamples/node-build-push-docker-ecr/blob/master/public/resources/images/console.jpg)
