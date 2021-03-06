# Fast and scalable differential expression analysis on single-cell RNA-seq data
diffxpy covers a wide range of differential expression analysis scenarios encountered in single-cell RNA-seq scenarios. The core ideas of diffxpy is to speed up the model fitting time, which is the run-time bottle-neck of differential expression analysis on models that require maximum likelihood estimators and that do not have closed form solutions thereof. This model fitting is performed in a separate package, batchglm. diffxpy exposes wrapper funtions to the user which perform the model fitting and the differential expression test. Advanced users can chose the between various hypothesis tests and can vary the model fitting hyperparameters. Fitting can be performed both on CPUs and on GPUs and can be parallelized.

# Worklows and API
Diffxpy supports workflows related to differential expression analysis. The functionalities of the workflows are structured in the API. To access these workflows, import diffxpy as follows `import diffxpy.api as de`. Currently, the following analytic strategies are implemented:

1. differential expression analysis in `de.test.*`
2. gene set enrichment analysis based on differential expression calls in `de.enrich.*`

The aforementioned workflows can be concatenated in pipelines and results can be shared via diffxpy data structures as explained in the individual functions and in the examples.
Refer to the documentation for details of the individual submodules.

# Installation
Please refer to the [documentation](https://diffxpy.rtfd.io).

# Tutorials
Please refer to the [documentation](https://diffxpy.rtfd.io).

# Documentation
The documentation of diffxpy is hosted [here](https://diffxpy.rtfd.io).
