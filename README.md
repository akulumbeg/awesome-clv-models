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
    - [Additional Valuable Sources](#additional-valuable-sources)
  - [Software Packages and Tools](#software-packages-and-tools)
    - [Python](#python)
    - [R](#r)

## Models and Papers

### Contractual Setting Models

Probabilistic models predicting churn and CLV in scenarios where transactions happen on fixed time periods, e.g. weekly, monthly.

  * **Beta-Geometric (BG)** (2007) - [[doi]](https://doi.org/10.1002/dir.20074) [[pdf]](https://faculty.wharton.upenn.edu/wp-content/uploads/2012/04/Fader_hardie_jim_07.pdf)
    > Fader, P. S., &amp; Hardie, B. G. S. (2007). How to Project Customer Retention. Journal of Interactive Marketing, 21(1), 76–90.

  * **Beta-discrete-Weibull (BdW)** (2018) - [[doi]](https://doi.org/10.1016/j.intmar.2018.01.002) [[pdf]](https://journals.sagepub.com/doi/pdf/10.1016/j.intmar.2018.01.002)
    > Fader, P. S., Hardie, B. G. S., Liu, Y., Davin, J., &amp; Steenburgh, T. (2018). “How to Project Customer Retention” Revisited: The Role of Duration Dependence. Journal of Interactive Marketing, 43, 1–16.


### Non-Contractual Setting Models (a.k.a. Buy 'Til You Die)

Probabilistic models predicting churn and CLV in scenarios where transactions appear spontaneously at any given time.

  * **Negative Binomial Distribution (NBD)** (1959) - [[doi]](https://doi.org/10.2307/2985810) [[pdf]](https://www.jstor.org/stable/pdf/2985810.pdf) 
    > Ehrenberg, A. S. (1959). The pattern of consumer purchases. Journal of the Royal Statistical Society. Series C (Applied Statistics), 8(1), 26–41.

  * **Pareto/NBD** (1987) - [[doi]](https://doi.org/10.1287/mnsc.33.1.1) [[pdf]](https://www.jstor.org/stable/pdf/2631608.pdf)
    > Schmittlein, D. C., Morrison, D. G., &amp; Colombo, R. (1987). Counting your customers: Who-are they and what will they do next? Management Science, 33(1), 1–24.

  * **BG/NBD** (2005) - [[doi]](https://doi.org/10.1287/mksc.1040.0098) [[pdf]](http://brucehardie.com/papers/018/fader_et_al_mksc_05.pdf) 
    > Fader, P. S., Hardie, B. G., &amp; Lee, K. L. (2005). “Counting your Customers” the Easy Way: An Alternative to the Pareto/NBD Model. Marketing Science, 24(2), 275–284.

  * **BG/NBD with time-invariant contextual factors** (2007) - [[doi]] [[pdf]]
    > Placeholder

  * **Pareto/NBD with time-invariant contextual factors** (2007) - [[doi]] [[pdf]]
    > Placeholder

  * **Pareto/NBD (Abe)** (2009) - [[doi]](https://doi.org/10.1287/mksc.1090.0502) [[pdf]](http://www.cirje.e.u-tokyo.ac.jp/research/dp/2008/2008cf537.pdf)
    > Abe, M. (2009). “Counting your Customers” One by One: A Hierarchical Bayes Extension to the Pareto/NBD Model. Marketing Science, 28(3), 541–553.

  * **BG/BB** (2010) - [[doi]] [[pdf]] 
    > Placeholder

  * **Gamma/Gompertz/NBD** (2012) - [[doi]] [[pdf]]    
    > Placeholder

  * **Pareto/GGG (GammaGammaGamma)** (2016) -  [[doi]](https://doi.org/10.1287/mksc.2015.0963) [[pdf]](http://www.reutterer.com/papers/platzer&reutterer_pareto-ggg_2016.pdf) 
    > Placeholder

  * **(M)BG/CNBD-k** (2021) - [[doi]](https://doi.org/10.1016/j.ijresmar.2020.09.002) [[pdf]](http://www.reutterer.com/papers/reutterer&platzer&schroeder_2021.pdf)
    > Reutterer, T., Platzer, M., &amp; Schröder, N. (2021). Leveraging Purchase Regularity for Predicting Customer Behavior the Easy Way. International Journal of Research in Marketing, 38(1), 194–215.  

  * **Gamma/Gompertz/NBD with time-invariant contextual factors** (2020) - [[doi]] [[pdf]]    
    > Placeholder

  * **Pareto/NBD with time-varying contextual factors** (2021) - [[doi]] [[pdf]]
    > Placeholder


MBG/NBD Batislam, E.P., M. Denizel, A. Filiztekin. 2007. Empirical validation and comparison of models for customer base analysis. International Journal of Research in Marketing 24(3) 201–209. \doi{10.1016/j.ijresmar.2006.12.005}

Pareto/NBD (HB) Ma, Shao-Hui, and Jin-Lan Liu. "The MCMC approach for solving the Pareto/NBD model and possible extensions." Natural Computation, 2007. ICNC 2007. Third International Conference on. Vol. 2. IEEE, 2007. \doi{10.1109/ICNC.2007.728}

Zhang 2015 RFM clumpiness


### Non-Probabilistic CLV Models

  * To be added (e.g. ML/DL approaches)
  * 

### Additional Valuable Sources

  * [Bruce Hardie's Notes](http://brucehardie.com/notes/)

## Software Packages and Tools

List of model implemenations and software tools in various programming languages.

### Python

  * [Lifetimes](https://github.com/CamDavidsonPilon/lifetimes) - Python implementation of BTYD models, namely BG, BG/BB, GG, MBG and Pareto/NBD

### R

  * [BTYD](https://github.com/ghuiber/BTYD) - The original R implementation of BTYD models, namely BG/BB, BG/NBD, P/NBD-GG
  * [BTYDplus](https://github.com/mplatzer/BTYDplus) - Extension of the BTYD package with NBD, MBG/NBD, (M)BG/CNBD-k, Pareto/NBD (HB), Pareto/NBD (Abe) and Pareto/GGG
  * [**CLVTools**](https://github.com/bachmannpatrick/CLVTools) ([web](https://www.clvtools.com)) - The most recent and optimized R package for BTYD models including the newest additions to the field
  * [foretell](https://github.com/sriharitn/foretell) - Implementation of contractual models by Fader, Hardie et al.

