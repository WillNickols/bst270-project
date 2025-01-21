# BST 270: Individual Project

This repository reproduces the figure from FiveThirtyEight's [Biden’s Cabinet Members Seem To Really Like Their Jobs](https://fivethirtyeight.com/features/biden-cabinet/).

## Installation

The GitHub can be cloned with TODO
```{bash}
git clone 
```

## Project Structure

A complete code reproduction attempt is available at `./code/hate_crimes_reproduction.qmd`. This notebook utilize [Quarto](https://quarto.org) and can be compiled via the command line and/or various IDEs/text editors (e.g. RStudio, VSCode, Jupyter, Neovim, Emacs). Refer to Quarto's [Get Started](https://quarto.org/docs/get-started/) and [Using R](https://quarto.org/docs/computations/r.html) documentation pages for more information. Quarto documents can also be compiled into multiple different file formats -- the repository also contains HTML, PDF, Tex, and Markdown files.

An image of the original plots is also provided in the `./data` directory.

### Getting Started

Use the following commands in Rstudio to install the package and open the
vignette containing the reproduced figures.
```
if (!require("devtools", quietly = TRUE))
    install.packages("devtools")
    
devtools::install_github("WillNickols/bst270-project", build_vignettes = TRUE,
    force = TRUE, dependencies = TRUE)
browseVignettes('bst270')
```

## Data

Once the pacakge is installed, the data set used for the reproduction analysis 
is available at `system.file(package="bst270","extdata","bad-drivers.csv")`. 
It is also available on [GitHub](https://github.com/fivethirtyeight/data/blob/master/bad-drivers/bad-drivers.csv).

# Bad Drivers

This folder contains data behind the story [Dear Mona, Which State Has The Worst Drivers?](http://fivethirtyeight.com/datalab/which-state-has-the-worst-drivers/)

Variable | Source
---|---------
`State` | N/A
`Number of drivers involved in fatal collisions per billion miles` | National Highway Traffic Safety Administration, 2012
`Percentage Of Drivers Involved In Fatal Collisions Who Were Speeding` | National Highway Traffic Safety Administration, 2009
`Percentage Of Drivers Involved In Fatal Collisions Who Were Alcohol-Impaired` | National Highway Traffic Safety Administration, 2012
`Percentage Of Drivers Involved In Fatal Collisions Who Were Not Distracted`	 | National Highway Traffic Safety Administration, 2012
`Percentage Of Drivers Involved In Fatal Collisions Who Had Not Been Involved In Any Previous Accidents` | National Highway Traffic Safety Administration, 2012
`Car Insurance Premiums ($)` | National Association of Insurance Commissioners, 2011
`Losses incurred by insurance companies for collisions per insured driver ($)` | National Association of Insurance Commissioners, 2010
