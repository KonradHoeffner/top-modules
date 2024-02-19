# Integrated TOP Framework Deployment

This is an unfinished experimental fork of the TOP Framework Deployment using Git submodules and a multi-module Maven project instead of the original architecture based on separate Docker images deployed on GitHub packages.
The reason for this experiment is that it is difficult and time-consuming to test changes in the original deployment especially when multiple components are to be changed in parallel.
This fork uses **[Git Submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)**, so clone it with the `--recursive` parameter, e.g. for SSH `git clone git@github.com:KonradHoeffner/top-modules.git --recursive`.
After checking out this repository, you need to copy `docker-compose.env.tpl` to `docker-compose.env` and adapt it.

```bash
git clone git@github.com:KonradHoeffner/top-modules.git --recursive
cp docker-compose.env.tpl docker-compose.env
docker compose pull
docker compose up --build
```

When updating with `git pull`, you also need to `git submodule update --recursive`.

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
