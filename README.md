# hssm_templates

Template code for running hierarchical regressions in hssm (https://lnccbrown.github.io/HSSM/). 

This code sets priors and starting points (for the sampler) and runs an example model of the cavanagh dataset (included in the hssm package).

Current hssm installation issues (10/10/23):
- numpy needs to be downgraded
- jax & jaxlib need to be downgraded

## Installation
```
conda create -n pyHSSM python=3.11.0
conda activate pyHSSM
pip install hssm
pip install numpy==1.25.0
pip install jaxlib==0.4.1 jax==0.4.1
```

 
