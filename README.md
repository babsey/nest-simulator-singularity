# nest-simulator-singularity


##### Requirement

- Singularity (>=2.6), see the documentation of Singularity offical website (https://sylabs.io/docs/)

##### Setup

Add bin folder into PATH environment.
```
export PATH=$PATH:<..>/nest-simulator-singularity/bin/
```
Please replace ```<..>``` with the location where you cloned this repository on your computer.

Hint: Add this line in .bashrc

Then execute a command to install singularity container with NEST simulator.
The latest version of NEST simulator is 2.18.0.
It will ask for password to get root rights to build singularity container.
```
nest-simulator build
```

To start shell with NEST Simulator
```
nest-simulator shell
```

To start ipython with NEST Simulator
```
nest-simulator ipython
```

To start notebook with NEST Simulator
```
nest-simulator notebook
```
