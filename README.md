# tsk
Trimmed Spearman-Karber Method. A simple nonparametric method to determine median effective doses (LD50, etc.) from dose-response curves. This package is based on the paper by Hamilton et al (1977, 1978).

To install, just type this in your R session:

    install.packages("devtools")
    install.packages("isotone")
    devtools::install_github(repo="brsr/tsk")

The package contains one function, `tsk`. Type `?tsk` in your R terminal for detailed help on the function. An example:

    > tsk( c(1, 10, 100, 1000), 20, c(0, 3, 17, 20) )
    $use.log.doses
    calculations done using the logs of the doses? 
                                              TRUE 
    $trim
    [1] 0
    $was.smoothed
    [1] FALSE
    $LD50
    [1] 31.62278
    $gsd
    geometric standard deviation of LD50 estimate 
                                         1.296928 
    $conf.int
    [1] 18.99717 52.63942
    attr(,"conf.level")
    [1] 0.95

This code was written several years ago. It runs and produces valid results, but may not be written in a contemporary R idiom.

This package was formerly located at https://r-forge.r-project.org/projects/tskarber/ . The R-forge project is being kept around to direct any existing users here. Any future updates will happen on Github.

## Citations

Hamilton, M. A.; Russo, R. C.; Thurston, R. V. Trimmed Spearman-Karber Method for Estimating Median Lethal Concentrations in Toxicity Bioassays. Enviro. Sci. Tech. 1977, 11 (7), 714-719. http://dx.doi.org/10.1021/es60130a004

Ibid, 1978, 12 (4), 417. http://dx.doi.org/10.1021/es60140a017
