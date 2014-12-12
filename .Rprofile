############################################################
## Options for knitr and Rmarkdown rendering
############################################################

## output directory for figures
if (require("knitr")) {
    opts_chunk$set(fig.path="results/figures/")
    opts_knit$set(base.dir=normalizePath(getwd()))
}

############################################################
## the following is credit to Jenny Bryan, for details see here:
## https://gist.github.com/jennybc/362f52446fe1ebc4c49f
RPROJ <- list(PROJHOME = normalizePath(getwd()))
attach(RPROJ)

cat('Project home directory is available as PROJHOME or via get("PROJHOME","RPROJ")\n')

rm(RPROJ)
############################################################
