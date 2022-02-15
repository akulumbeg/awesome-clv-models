# CLV Models and More

This list contains a curated, ever-growing collection of papers and repositories about modelling and prediction of customer churn and customer lifetime value.

Contributions and feedback are more than welcome.

## Table of Contents
- [CLV Models and More](#clv-models-and-more)
  - [Table of Contents](#table-of-contents)
  - [Models and Papers](#models-and-papers)
    - [Contractual Setting Models](#contractual-setting-models)
    - [Non-Contractual Setting Models (a.k.a. Buy 'Til You Die)](#non-contractual-setting-models-aka-buy-til-you-die)
    - [Extensions](#extensions)
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

  * **BG/NBD with time-invariant contextual factors** (2007) - [[pdf]](http://brucehardie.com/notes/019/time_invariant_covariates.pdf)
    > Fader, P. S., &amp; Hardie, B. G. S. (2007). Incorporating Time-Invariant Covariates into the Pareto/NBD and BG/NBD Models

  * **Pareto/NBD with time-invariant contextual factors** (2007) - [[pdf]](http://brucehardie.com/notes/019/time_invariant_covariates.pdf)
    > Fader, P. S., &amp; Hardie, B. G. S. (2007). Incorporating Time-Invariant Covariates into the Pareto/NBD and BG/NBD Models

  * **MBG/NBD** (2007) - [[doi]](https://doi.org/10.1016/j.ijresmar.2006.12.005) [[pdf]](https://www.sciencedirect.com/science/article/pii/S0167811607000171/pdfft?isDTMRedir=true&download=true)
    > Batislam, E. P., Denizel, M., &amp; Filiztekin, A. (2007). Empirical validation and comparison of models for customer base analysis. International Journal of Research in Marketing, 24(3), 201–209.  

  * **Pareto/NBD (HB)** (2007) - [[doi]](https://doi.org/10.1109/ICNC.2007.728) [[pdf]](https://csdl-downloads.ieeecomputer.org/proceedings/icnc/2007/2875/02/28750505.pdf?Expires=1644938774&Policy=eyJTdGF0ZW1lbnQiOlt7IlJlc291cmNlIjoiaHR0cHM6Ly9jc2RsLWRvd25sb2Fkcy5pZWVlY29tcHV0ZXIub3JnL3Byb2NlZWRpbmdzL2ljbmMvMjAwNy8yODc1LzAyLzI4NzUwNTA1LnBkZiIsIkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTY0NDkzODc3NH19fV19&Signature=tmHnuo9llkidSnMA5Trd-FaAr70V3OGKFcw9pevnN8vwZrlsdUenRNcR8AVqEtGjSGEmQ~D7VKRB8FYP9Fok8qPbLWK3ziVVgPwbuBsD-CCVnE7b13fDKLaCVQlZesPWOa5wKadUWoP34NTL3~Q-HqqxaLlSurMaBfpYHpEpFQHykOmJk~98khgRuoqWnGoDLowQHF3GDixbdP1Fr0hwUQVzbvGI4sEZRJc0iZFcjbQPCSRVEGF8xQL0A2H7atsDcZue2psEiwlZHIhsrjqLD4Ezt5OeVi7kCuXvYhsX71EGqovefuR0Crg~ZPhuZLP4Hwn8MMHoCZXVzZYpKmb58g__&Key-Pair-Id=K12PMWTCQBDMDT)
    > Ma, S.-H., &amp; Liu, J.-L. (2007). The MCMC approach for solving the pareto/NBD model and possible extensions. Third International Conference on Natural Computation (ICNC 2007).

  * **Pareto/NBD (Abe)** (2009) - [[doi]](https://doi.org/10.1287/mksc.1090.0502) [[pdf]](http://www.cirje.e.u-tokyo.ac.jp/research/dp/2008/2008cf537.pdf)
    > Abe, M. (2009). “Counting your Customers” One by One: A Hierarchical Bayes Extension to the Pareto/NBD Model. Marketing Science, 28(3), 541–553.

  * **BG/BB (Beta-Geometric/Beta-Binomial)** (2010) - [[doi]](https://doi.org/10.1287/mksc.1100.0580) [[pdf]](http://www.brucehardie.com/papers/020/fader_et_al_mksc_10.pdf) 
    > Fader, P. S., Hardie, B. G., &amp; Shang, J. (2010). Customer-base analysis in a discrete-time noncontractual setting. Marketing Science, 29(6), 1086–1108.

  * **Gamma/Gompertz/NBD** (2012) - [[doi]](https://doi.org/10.1287/mnsc.1110.1461) [[pdf]](https://pubsonline.informs.org/doi/pdf/10.1287/mnsc.1110.1461)
    > Bemmaor, A. C., &amp; Glady, N. (2012). Modeling purchasing behavior with sudden “death”: A flexible customer lifetime model. Management Science, 58(5), 1012–1021. 

  * **Pareto/GGG (GammaGammaGamma)** (2016) -  [[doi]](https://doi.org/10.1287/mksc.2015.0963) [[pdf]](http://www.reutterer.com/papers/platzer&reutterer_pareto-ggg_2016.pdf) 
    > Platzer, M., &amp; Reutterer, T. (2016). Ticking away the moments: Timing regularity helps to better predict customer activity. Marketing Science, 35(5), 779–799. 

  * **(M)BG/CNBD-k ** (2021) - [[doi]](https://doi.org/10.1016/j.ijresmar.2020.09.002) [[pdf]](http://www.reutterer.com/papers/reutterer&platzer&schroeder_2021.pdf)
    > Reutterer, T., Platzer, M., &amp; Schröder, N. (2021). Leveraging Purchase Regularity for Predicting Customer Behavior the Easy Way. International Journal of Research in Marketing, 38(1), 194–215.  

  * **Pareto/NBD with time-varying contextual factors** (2021) - [[doi]](https://doi.org/10.1287/mksc.2020.1254) [[pdf]](https://www.zora.uzh.ch/id/eprint/197236/1/mksc.2020.1254.pdf)
    > Bachmann, P., Meierer, M., &amp; Näf, J. (2021). The role of time-varying contextual factors in latent attrition models for customer base analysis. Marketing Science, 40(4), 783–809.


### Extensions
  * **RFM to RFMC (Clumpiness)** (2015) - [[doi]](https://doi.org/10.1287/mksc.2014.0873) [[pdf]](https://pubsonline.informs.org/doi/pdf/10.1287/mksc.2014.0873)
    > Zhang, Y., Bradlow, E.T., & Small, D. S. (2015). Predicting Customer Value Using Clumpiness: From RFM to RFMC. Marketing Science, 34(2), 195-208.

### Non-Probabilistic CLV Models

  * To be added (e.g. ML/DL approaches)

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
