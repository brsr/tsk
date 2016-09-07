# tsk
Trimmed Spearman-Karber Method. A simple nonparametric method to determine median effective doses (LD50, etc.) from dose-response curves. This package is based on the paper by Hamilton et al (1977, 1978).

To install, just type this in your R session:

    install.packages("isotone")
    devtools::install_github(repo="brsr/tsk")

This code was written several years ago. It runs and produces valid results, but may not be written in a contemporary R idiom.

This package was formerly located at https://r-forge.r-project.org/projects/tskarber/ . The R-forge project is being kept around to direct existing users (all 5 of them) here. Any future updates will happen on Github.

## Citations

Hamilton, M. A.; Russo, R. C.; Thurston, R. V. Trimmed Spearman-Karber Method for Estimating Median Lethal Concentrations in Toxicity Bioassays. Enviro. Sci. Tech. 1977, 11 (7), 714-719. http://dx.doi.org/10.1021/es60130a004

Ibid, 1978, 12 (4), 417. http://dx.doi.org/10.1021/es60140a017
