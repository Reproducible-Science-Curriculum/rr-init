Reproducible Research Project Initialization
=======

Research project initialization and organization following reproducible research guidelines.

Overview
--------

    project
    |- doc/            # documentation for the study
    |  +- paper/       # manuscript(s), whether generated or not
    |
    |- data            # raw and primary data, are not changed once created 
    |  |- raw/         # raw data, will not be altered
    |  +- clean/       # cleaned data, will not be altered once created
    |
    |- code/           # any programmatic code
    |- results         # all output from workflows and analyses
    |  |- figures/     # graphs, likely designated for manuscript figures
    |  +- pictures/    # diagrams, images, and other non-graph graphics
    |
    |- scratch/        # temporary files that can be safely deleted or lost
    |- README          # the top level description of content
    |- study.Rmd       # executable Rmarkdown for this study, if applicable
    |- Makefile        # executable Makefile for this study, if applicable
    |- study.Rproj     # RStudio project for this study, if applicable
    |- datapackage.json # metadata for the (input and output) data files 

How to use
----------

* Create a new directory for your project.
* Download the [latest release] of this repository, and unzip it in the directory you just created.
* Open this document in an editor. Change the first line to reflect the title of your research study, and delete the rest of the content in this file. You can, but are not obligated to keep the Acknowledgements section.
* Delete the LICENSE.md file, unless it will also apply to your project. (However, it probbaly will not to all of it.)
* Go forth and experiment, keeping files in their appropriate places.

To the extent possible under law, the author(s) of this template have dedicated all copyright and related and neighboring rights to it to the public domain worldwide under the [CC0 Public Domain Dedication]. The template and all other content in the [rr-init repository] is distributed without any warranty.

Key concepts and goals
----------------------

See [Noble 2009] for a full description of and argument for the principle template structure. Some concepts and goals that guided this work:
* (Good) There is a folder for the raw data, which do not get altered, or intermixed with data that is the result of manual or programmatic manipulation. I.e., derived data is kept separate from raw data, and raw data are not duplicated.
* (Good) Code is kept separate from data.
* (Better) Manuscript production output is kept separate from everything else.
* (Good) There is a scratch directory for experimentation. Everything in the scratch directory can be deleted at any time without negative impact. 
* (Better) There should be a `README` in evey directory, describing the purpose of the directory and its contents.
* (Best) There is a top-level `Makefile` or [Rmarkdown] file that documents the computational study in executable form. Those files may call out to other `Makefile`'s or `.Rmd` files in subdirectories.
* (Best) There is a formal metadata descriptor at the root of the package that describes all the important input and output data files.
* (Meta) The template structure should have no special software or skill prerequisites to install. Specifically, deploying the template structure should not require installing git, or using the command line.

Acknowledgements
----------------

The initial file and directory structure of this project was developed by a group of participants in the Reproducible Science Curriculum Workshop, held at [NESCent] in December 2014. The structure is based on, and heavily follows the one proposed by [Noble 2009], with a few but small modifications.

[rr-init repository]: https://github.com/Reproducible-Science-Curriculum/rr-init
[latest release]: https://github.com/Reproducible-Science-Curriculum/rr-init/releases/latest
[NESCent]: http://nescent.org
[Rmarkdown]: http://rmarkdown.rstudio.com/
[Noble 2009]: http://dx.doi.org/10.1371/journal.pcbi.1000424
[CC0 Public Domain Dedication]: http://creativecommons.org/publicdomain/zero/1.0/
