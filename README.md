Node.js container based on Alpine Linux OS

### Tags:
* [`6.8` *(6.8/Dockerfile)*](https://github.com/adityasetiono/node/blob/master/6.8/Dockerfile)
* [`7.2`, `latest` *(7.2/Dockerfile)*](https://github.com/adityasetiono/node/blob/master/7.2/Dockerfile)
* [`7.2-slim`, `slim` *(slim/Dockerfile)*](https://github.com/adityasetiono/node/blob/master/slim/Dockerfile)

### Installed Packages:
* sails
* forever
* yarn
* aglio

### Usage:
To use the package locally, create a bash file in `/usr/local/bin` and add the docker run script like so.
##### `/usr/local/bin/node`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest node $@
```
`$ node --version`
`v6.8.0`
***
##### `/usr/local/bin/npm`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest npm $@
```
`$ npm --version`
`3.10.8`
***
##### `/usr/local/bin/sails`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest sails $@
```
`$ sails --version`
`0.12.7`
***
##### `/usr/local/bin/yarn`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest yarn $@
```
`$ yarn --version`
`0.15.0`
***
##### `/usr/local/bin/forever`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest forever $@
```
`$ forever --version`
`0.14.2`
***
##### `/usr/local/bin/aglio`
```
#!/bin/sh
export PATH=/sbin:/bin:/usr/sbin:/usr/bin:/usr/local/sbin:/usr/local/bin
docker run --rm --name my-running-script -v $(pwd):/usr/src/app -w /usr/src/app chilongqua/node:latest aglio $@
```
`$ aglio --version`
`aglio 2.2.1`
`olio 1.6.3`
***
