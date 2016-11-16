[![N|Solid](./imgs/nsolid.png)](https://nodesource.com/products/nsolid)

N|Solid Docker Images
=====================

Welcome to the home for the source code of the N|Solid Docker Images!

# Images

This repository is used to build and push the following 4 images to the Docker Hub:

* [nodesource/nsolid](https://hub.docker.com/r/nodesource/nsolid)
* [nodesource/nsolid-console](https://hub.docker.com/r/nodesource/nsolid-console)
* [nodesource/nsolid-storage](https://hub.docker.com/r/nodesource/nsolid-storage)
* [nodesource/nsolid-cli](https://hub.docker.com/r/nodesource/nsolid-cli)

If you are looking for documentation on how to use these images, checkout our the official [docs](https://docs.nodesource.com)!

### Building Images

```bash
NSOLID_VERSION=2.0.1 make build 
```

### Publishing Images

```bash
DOCKER_REGISTRY=username NSOLID_VERSION=2.0.1 make publish
```

### Cleaning up

```bash
NSOLID_VERSION=2.0.1 make clean # removes download directories `nsolid-bundle-*`
NSOLID_VERSION=2.0.1 make cleanall # runs `make clean` and removes all docker images with label=nodesource=nsolid
```

# Contributing

To submit a bug report, please create an [issue at GitHub](https://github.com/nodesource/docker-nsolid/issues/new).

If you'd like to contribute code to this project, please read the
[CONTRIBUTING.md](https://github.com/nodesource/docker-nsolid/blob/master/CONTRIBUTING.md) document. It contains a breif overview of this repo.

# Authors and Contributors

<table><tbody>
  <tr>
    <th align="left">William Blankenship</th>
    <td><a href="https://github.com/retrohacker">GitHub/retrohacker</a></td>
    <td><a href="https://twitter.com/retrohack3r">Twitter/@retrohack3r</a></td>
  </tr>
  <tr>
    <th align="left">Daniel Aristizabal</th>
    <td><a href="https://github.com/cronopio">GitHub/cronopio</a></td>
    <td><a href="https://twitter.com/cronopio2">Twitter/@cronopio2</a></td>
  </tr>
  <tr>
    <th align="left">Joe McCann</th>
    <td><a href="https://github.com/joemccann">GitHub/joemccann</a></td>
    <td><a href="https://twitter.com/joemccann">Twitter/@joemccann</a></td>
  </tr>
  <tr>
    <th align="left">Patrick Mueller</th>
    <td><a href="https://github.com/pmuellr">GitHub/pmuellr</a></td>
    <td><a href="https://twitter.com/pmuellr">Twitter/@pmuellr</a></td>
  </tr>
</tbody></table>

# License & Copyright

**docker-nsolid** is Copyright (c) 2016 NodeSource and licensed under the
MIT license. All rights not explicitly granted in the MIT license are reserved.
See the included [LICENSE.md](https://github.com/nodesource/docker-node/blob/master/LICENSE.md) file for more details.

The projects contained within the **docker-nsolid** images maintain their own Licenses.
