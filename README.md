# hssm_templates

Template code for running hierarchical regressions in hssm (https://lnccbrown.github.io/HSSM/). Developed with generous help from Alexander Fengler (http://alexanderfengler.github.io/about/) 

This code sets priors and starting points (for the sampler) and runs an example model of the cavanagh dataset (included in the hssm package).

## Contents

**DDM_LAN_Likelhood_NutsSampler.ipynb**
    - Fits a DDM using the LAN likelihood and nuts_numpyro sampler

**DDM_Analytical_Likelihood_SliceSampler.ipynb**
    - Fits a DDM using the analytical likelihood and a slice sampler
    - This should be the same as using HDDM (not confirmed yet)

## Issues

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

## TO DO

- Add code for analytical likelihood
    - Add exp link function for threshold
    - Add logit link function for bias
    - Do inverses for the two parameters in the model object

- Add instructions on how to run on GPU 



 
