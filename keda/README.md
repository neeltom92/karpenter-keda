# Installation

1. Installation is pretty straightforward using helm : https://keda.sh/docs/2.0/deploy/#helm
this installation is referred from : https://gist.github.com/vfarcic/2dad051fe41bd2bbcf94eda74386ce49
2. cooldownPeriod has no effect  [here](https://github.com/kedacore/keda/issues/737)
as KEDA manages 0 <-> 1 and HPA 1 <-> N scaling
3. so if there are 4 pods (scale down to 1 will happen after 15 mins only(4*5-5) )
4. attached a sample deployment and keda for CPU file.
