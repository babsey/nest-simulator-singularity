# NEST Simulator Singularity

See the offical documentation of Singularity page (https://sylabs.io/docs/)

## Installation

#### Requirements

- Singularity (>=3.0)

##### 1. Clone working copy from the repos

```
git clone https://github.com/babsey/nest-simulator-singularity
```

##### 2. Make nest-simulator-singularity executable visible.

Add `bin` folder into PATH environment.

```
export PATH=$PATH:$PWD/bin/
```

Hint: Add `PATH` definition for NEST Simulator Singularity command in `.bashrc`.

## Usage

##### 1. Build a singularity image containing NEST Simulator

The latest version of NEST simulator is 3.0.
It will ask for password to get root rights to build Singularity container.

```
nest-simulator-singularity build
```

##### 2. Start a Singularity image containing NEST Simulator

To start shell with NEST Simulator.

```
nest-simulator-singularity shell
```

To start ipython with NEST Simulator.

```
nest-simulator-singularity ipython
```

To start notebook with NEST Simulator.

```
nest-simulator-singularity notebook
```

To start API Server of NEST Simulator (3.0 or newer).

```
nest-simulator-singularity api
```

##### Other NEST version

or execute command with specific version of NEST Simulator (See files in [./recipes](./recipes)).

```
nest-simulator-singularity ... -v 3.0
```
