# nest-singularity


##### Requirement

- Singularity (>=2.6), see the documentation of Singularity offical website (https://sylabs.io/docs/)

##### Setup

Add bin folder into PATH environment.
```
export PATH=$PATH:<..>/nest-singularity/bin/
```
Please replace ```<..>``` with the location where you cloned this repository on your computer.

Hint: Add this line in .bashrc

Then execute a command to install singularity container with NEST simulator. The latest version of NEST simulator is 2.18.0.
```
nest-singularity build 2.18.0
```

To start notebook
```
nest-singularity notebook 2.18.0
```

To start ipython3
```
nest-singularity interactive 2.18.0
```

To execute python script in container
```
nest-singularity script 2.18.0 <file>
```
