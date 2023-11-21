# Integrated TOP Framework Deployment

This is an unfinished experimental fork of the TOP Framework Deployment using Git submodules and a multi-module Maven project instead of the original architecture based on separate Docker images deployed on GitHub packages.
The reason for this experiment is that it is difficult and time-consuming to test changes in the original deployment especially when multiple components are to be changed in parallel.
After checking out this repository, you need to:

```bash
git submodule update --init
```

Original README below.

# TOP Framework Deployment
This repository contains deployment instructions and resources for the TOP Framework.

The TOP Framework consists of:

* **Frontend:** [Vue.js](https://vuejs.org) and [Quasar](https://quasar.dev) based Single-Page Application ([top-frontend](https://github.com/Onto-Med/top-frontend))
* **Backend:** [Spring Boot Resource Server](https://docs.spring.io/spring-security/reference/servlet/oauth2/resource-server/index.html) ([top-backend](https://github.com/Onto-Med/top-backend))

## State of the Project
The TOP Framework is currently under heavy development. Usage in a production environment is not yet recommended.

A public demo instance is available at: https://top.imise.uni-leipzig.de

## Usage
See https://onto-med.github.io/top-deployment.

## License
The TOP Framework is licensed under the [MIT license](LICENSE).
