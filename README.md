# CLV Models and More

This list contains a curated, ever-growing collection of papers and repositories about modelling and prediction of customer churn and customer lifetime value.

Contributions and feedback are more than welcome.

## Table of Contents
- [CLV Models and More](#clv-models-and-more)
  - [Table of Contents](#table-of-contents)
  - [Models and Papers](#models-and-papers)
    - [Contractual Setting Models](#contractual-setting-models)
    - [Non-Contractual Setting Models (a.k.a. Buy 'Til You Die)](#non-contractual-setting-models-aka-buy-til-you-die)
    - [Non-Probabilistic CLV Models](#non-probabilistic-clv-models)
  - [Software Packages and Tools](#software-packages-and-tools)
    - [Python](#python)
    - [R](#r)

## Models and Papers

### Contractual Setting Models

Probabilistic models predicting churn and CLV in scenarios where transactions happen on fixed time periods, e.g. weekly, monthly.

  * **Beta-Geometric** - [[doi]](https://doi.org/10.1002/dir.20074) [[pdf]](https://faculty.wharton.upenn.edu/wp-content/uploads/2012/04/Fader_hardie_jim_07.pdf)
    > Fader, P. S., &amp; Hardie, B. G. S. (2007). How to Project Customer Retention. Journal of Interactive Marketing, 21(1), 76–90.

  * **Beta-discrete-Weibull** [[doi]](https://doi.org/10.1016/j.intmar.2018.01.002) [[pdf]]()
    > Fader, P. S., Hardie, B. G. S., Liu, Y., Davin, J., &amp; Steenburgh, T. (2018). “How to Project Customer Retention” Revisited: The Role of Duration Dependence. Journal of Interactive Marketing, 43, 1–16.


### Non-Contractual Setting Models (a.k.a. Buy 'Til You Die)

Probabilistic models predicting churn and CLV in scenarios where transactions appear on spontaneously at any given time.

  * NBD - 
  * 1987 - Pareto/NBD  
  * 2005 - BG/NBD  
  * 2007 - BG/NBD with time-invariant contextual factors  
  * 2007 - Pareto/NBD with time-invariant contextual factors  
  * Pareto/NBD (Abe) - 
  * 2010 - BG/BB  
  * 2016 - Pareto/GammaGammaGamma (paper) -   

Acronyms:
  * NBD - Negative Binomial Distribution
  * BB - Beta Binomial
  * BG - Beta Geometric
  * GGG - Gamma-Gamma-Gamma

### Non-Probabilistic CLV Models

  * 

## Software Packages and Tools

List of model implemenations and software tools in various programming languages.

### Python

  * [Lifetimes](https://github.com/CamDavidsonPilon/lifetimes) - Python implementation of BTYD models, namely BG, BG/BB, GG, MBG and Pareto/NBD

### R

  * [BTYD](https://github.com/ghuiber/BTYD) - The original R implementation of BTYD models, namely BG/BB, BG/NBD, P/NBD-GG
  * [BTYDplus](https://github.com/mplatzer/BTYDplus) - Extension of the BTYD package with NBD, MBG/NBD, (M)BG/CNBD-k, Pareto/NBD (HB), Pareto/NBD (Abe) and Pareto/GGG
  * [**CLVTools**](https://github.com/bachmannpatrick/CLVTools) ([web](https://www.clvtools.com)) - The most recent and optimized R package for BTYD models including the newest additions to the field
  * [foretell](https://github.com/sriharitn/foretell) - Implementation of contractual models by Fader, Hardie et al.

