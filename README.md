# Covid Data Visualization

#### Data Source: Mexico CDC

This is my attempt to visualize Covid data and the models

Steps to remember: - Create a project with local git - Then use the following command to create a git repo on GitHub: - R command `usethis::use_github()`

If you have not connected your GitHub account with RStudio use the following commands to set it up:

To create a token

`usethis::create_github_token()`

Then register your token with RStudio using the following command:

`gitcreds::gitcreds_set()` and paste the token

Ref: <https://happygitwithr.com/>

### Note about dashboards and tools:

-   If you are doing a static article, blog, book or a dashboard then Quarto is best because it has good layout options. Combine with `bslib`, you can make very good static dashboard using Quarto.

-   If you have lot of reactive dashboard then you need shiny, you can use shiny inside Quarto but it is a bit hard. The issue with Shiny is that you need to write a lot of code to set it up but it works.

-   `flexdashboard` package is a compromise between Shiny and Quarto. I recommend using it for moderate level dashboards.

### A Point about Tabsets

-   In `flexdashboard` within a single tab the plots are arranged vertically (annoying). See <https://github.com/rstudio/flexdashboard/issues/265>
-   Use `gridExtra` or `patchwork` for more flexibility.
