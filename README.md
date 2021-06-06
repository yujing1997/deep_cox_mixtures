# Deep Cox Mixtures
#### _Chirag Nagpal<sup>1,2</sup> Steve Yadlowsky<sup>1</sup>, Negar Rostamzadeh<sup>1</sup> and Katherine Heller<sup>1</sup>_

#### _<sup>1</sup>Google Brain Team_, _<sup>2</sup>Carnegie Mellon University_

This repository contains code for the NeurIPS 2020, ML4H paper: 
[Deep Cox Mixtures for Survival Regression](https://arxiv.org/abs/2101.06536)

### Installation

To download and run Deep Cox Mixtures:

```console
foo@bar:~$ git clone https://github.com/chiragnagpal/deep_cox_mixtures.git
foo@bar:~$ cd deep_cox_mixtures
foo@bar:~$ pip install -r requirements.txt
```


### Usage

To run DCM on a standard survival analysis dataset like SUPPORT, please see the following
example notebook:


To run the original experiments from the paper, please use: 
```
from dcm import deep_cox_mixture
results = deep_cox_mixture.experiment(dataset='SUPPORT', prot_att='race', groups=('white', 'other'))
deep_cox_mixture.display_results(results)
```
### Requirements
`dcm` depends on `tensorflow2` and `scikit-survival`, 

Running baseline models for comparison requires `lifelines`, `pycox` and `dsm`
