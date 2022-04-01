# scopes-chipmunk2d

## Installation

The module is under `src/chipmunk2d`. You can copy this subtree into your
project and then add it to the `package.path` in your Scopes
`_project.sc` file.

### With Spack

This module is available as the `scopes-chipmunk2d` package in the
[snailpacks](https://github.com/salotz/snailpacks) repository. This will pull in the necessary dependencies
including Scopes.

```sh
  spack install scopes-chipmunk2d
```

See the [snailpacks](https://github.com/salotz/snailpacks) documentation for more best practices of installing.

## Development Environment

We use [Spack](https://spack.io/) to install dependencies. First install Spack.

Then you'll need our custom repo of build recipes:

```sh
  mkdir -p `/.spack/repos
  git clone git@github.com:salotz/snailpacks.git `/.spack/repos/snailpacks
  spack repo add `/resources/spack-repos/snailpacks
```

Then you need to create an environment in this folder that will
contain the headers and libraries etc.

```sh
  spack env create -d .
```

Activate the environment (i.e. set the environment variables
appropriately) and install the packages:

```sh
  spacktivate .
  spack install
```

To exit the environment (i.e. unset the env variables):

```sh
  despacktivate
```
