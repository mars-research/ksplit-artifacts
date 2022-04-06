# Artifact Evaluation - OSDI'22

This documentation contains steps necessary to reproduce the artifacts for our
paper titled **KSplit: Automating Device Driver Isolation**.

All the experiments are evaluated on a Dell PowerEdge R820 machine on the
[Emulab Infrastructure](https://www.emulab.net/apt/show-hardware.php?type=d820)


## Setting up the hardware

* Create an account on [Cloudlab](https://www.cloudlab.us/) and login.

### Configuring the experiment
* Start an experiment by creating a node of type `d820`

* Create an experiment from the below github profile repository. The profile
  comes pre-installed with LVDs kernel for testing the drivers. (TODO)
```
https://github.com/arkivm/cloudlab-profiles
```

* Everything should be setup automatically at `/opt/ksplit/`

## Experiments

### Table2

* Compile Program dependence graph from the cloned sources
```
cd /opt/ksplit/pdg
mkdir build && cd build
cmake ..
make
```
* Run a simple test program
```

```
