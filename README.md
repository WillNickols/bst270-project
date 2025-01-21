# BST 270: Individual Project

This repository reproduces the figures from FiveThirtyEight's [Dear Mona, Which State Has The Worst Drivers?](https://fivethirtyeight.com/features/which-state-has-the-worst-drivers/). Doing so will utilize data from the National Highway Traffic Safety Administration (2009, 2012) and National Association of Insurance Commissioners (2010, 2011).

### Getting Started

Use the following commands in Rstudio to install the package and its 
dependencies and open the vignette containing the reproduced figures. 
```
if (!require("devtools", quietly = TRUE))
    install.packages("devtools")
    
devtools::install_github("WillNickols/bst270-project", build_vignettes = TRUE,
    force = TRUE, dependencies = TRUE)
browseVignettes('bst270')
```

## Project Structure

The reproduction is available in the included vignette, which can be viewed 
with `browseVignettes('bst270')` or 
`vignette("bad_drivers_reproduction", package="bst270")`. An image of the 
original article is provided in the `inst/extdata` directory.

To view the source code, the whole package can be cloned from 
`https://github.com/WillNickols/bst270-project/`.

## Data

Once the pacakge is installed, the data set used for the reproduction analysis 
is available at `system.file(package="bst270","extdata","bad-drivers.csv")`. 
It is also available on [GitHub](https://github.com/fivethirtyeight/data/blob/master/bad-drivers/bad-drivers.csv).

The schema and supporting sources are below:

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
