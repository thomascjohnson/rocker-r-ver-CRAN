# Precompiled CRAN for rocker/r-ver

Many an R developer has suffered through the agony of long build times of source packages in Docker. In some cases, this can make operating infrastructure dependent on Docker images containing many R packages a difficult endeavor. Have no fear, rocker/r-ver CRAN is here.

## Usage
Simply add this Github repository's user content url to your repositories:
```
options(repos = c("https://raw.githubusercontent.com/thomascjohnson/rocker-r-ver-CRAN/latest/", getOption("repos")))
```

Then use R and `install.packages` just as you normally would. As long as you're in the rocker/r-ver:latest container, packages will install in a flash.
