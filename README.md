# Multi-ancestry finemapping of gene clusters implicated in cardiovascular disease and mental health

## Analysis plan

1. Extract region of interest from MDD sumstats.
2. Liftover MDD sumstats to build 38.
3. Multi-ancestry finemapping using [SuSiEx](https://github.com/getian107/SuSiEx) with standard reference panels.
4. Run [PolyFun with precomputed priors](https://github.com/omerwe/polyfun/wiki/1.-Computing-prior-causal-probabilities-with-PolyFun#polyfun-approach-1-using-precomputed-prior-causal-probabilities-based-on-a-meta-analysis-of-15-uk-biobank-traits).
4. Extract region of interest from WGS dataset
5. QC WGS dataset
6. Compute [PolyFun priors non-parametrically](https://github.com/omerwe/polyfun/wiki/1.-Computing-prior-causal-probabilities-with-PolyFun#polyfun-approach-3-computing-prior-causal-probabilities-non-parametrically) using WGS datasets.
7. Perform [functionally-informed finemapping with PolyFun](https://github.com/omerwe/polyfun/wiki/3.-Functionally-informed-fine-mapping-with-finemapper) using different priors.

## Acknowledgments

Project supported by **REA4 Pump Priming Award** (RE/24/130012).
