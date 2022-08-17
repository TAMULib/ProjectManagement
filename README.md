<a name="readme-top"></a>
[![Service Build Status][service-build-badge]][service-build-status]
[![Client Build Status][client-build-badge]][client-build-status]
[![Service overage Status][service-coverage-badge]][service-coverage-status]
[![Client overage Status][client-coverage-badge]][client-coverage-status]

# Project Management App

The *Project Management App*, consisting of a service back-end and a client front-end, is developed and maintained by [Texas A&M University Libraries][tamu-library].

Using this repository requires loading a submodule, such as one of these methods:
```shell
# Method 1: Checkout with submodule recursion.
git clone https://github.com/TAMULib/ProjectManagement.git ProjectManagement --recurse-submodules

# Method 2: Initialize submodule for already checked out repository.
cd ProjectManagement/
git submodule init
```

<div align="right">(<a href="#readme-top">back to top</a>)</div>


## Deployment

A quick and easy deployment method using `docker-compose` is described in the [Deployment Guide][deployment-guide].

For _advanced use cases_, or when `docker-compose` is unavailable, the use of `docker` or `npm`/`mvn` is also described in the [Deployment Guide][deployment-guide].

Deployment, in general, may look something like this:

```shell
cp example.env .env
cp example.env.client .env.client
cp example.env.service .env.service

# Make any changes to the .env, .env.client, and .env.service files before here.
docker-compose up
```

<div align="right">(<a href="#readme-top">back to top</a>)</div>


## Additional Resources

- [Contributors Documentation][contribute-guide]
- [Deployment Documentation][deployment-guide]
- [API Documentation][api-docs]

Please feel free to file any issues concerning *Project Management App* to the issues section of the repository.

Any questions concerning *Project Management App* can be directed to helpdesk@library.tamu.edu.

Copyright © 2022 Texas A&M University Libraries under the [MIT License][license].

<div align="right">(<a href="#readme-top">back to top</a>)</div>


<!-- LINKS -->
[service-build-status]: https://github.com/TAMULib/ProjectManagementService/actions?query=workflow%3ABuild
[service-build-badge]: https://github.com/TAMULib/ProjectManagementService/workflows/Build/badge.svg
[service-coverage-status]: https://coveralls.io/github/TAMULib/ProjectManagementService
[service-coverage-badge]: https://coveralls.io/repos/github/TAMULib/ProjectManagementService/badge.svg

[client-build-status]: https://github.com/TAMULib/ProjectManagementUI/actions?query=workflow%3ABuild
[client-build-badge]: https://github.com/TAMULib/ProjectManagementUI/workflows/Build/badge.svg
[client-coverage-status]: https://coveralls.io/github/TAMULib/ProjectManagementUI
[client-coverage-badge]: https://coveralls.io/repos/github/TAMULib/ProjectManagementUI/badge.svg

[tamu-library]: http://library.tamu.edu
[api-docs]: https://tamulib.github.io/ProjectManagementService

[deployment-guide]: DEPLOYING.md
[contribute-guide]: CONTRIBUTING.md
[license]: LICENSE
