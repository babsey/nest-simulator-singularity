# nest-singularity


#### Requirement

- Singularity (>=2.6), see the documentation of Singularity offical website (https://sylabs.io/docs/)

#### Setup

##### 1. Clone working copy from the repos
```
git clone https://github.com/babsey/nest-singularity
```

##### 2. Make nest-simulator executable visible.

Add bin folder into PATH environment.
```
export PATH=$PATH:<..>/nest-singularity/bin/
```
Please replace ```<..>``` with the location where you cloned the working copy on your computer.

Hint: Add this line in .bashrc


#### Usage

##### 1. Build a singularity image containing NEST Simulator

The latest version of NEST simulator is 2.18.0.
It will ask for password to get root rights to build singularity container.
```
nest-singularity build
```

##### 2. Start a singularity image containing NEST Simulator

To start shell with NEST Simulator
```
nest-singularity shell
```

To start ipython with NEST Simulator
```
nest-singularity ipython
```

To start notebook with NEST Simulator
```
nest-singularity notebook
```

##### Other NEST version

or execute command with specific version of NEST Simulator (See files in [./recipes](./recipes)).
```
nest-singularity ... -v v2.18.0
```
