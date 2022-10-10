# Name of App *(Give your app a short and informative title. Please adhere to our convention of Title Case without hyphens (e.g. My New App))*

MoveApps

Github repository: *github.com/yourAccount/Name-of-App* *(the link to the repository where the code of the app can be found must be provided)*

## Description
*Enter here the short description of the App that might also be used when filling out the description when submitting the App to Moveapps. This text is directly presented to Users that look through the list of Apps when compiling Workflows.*

## Documentation
*Enter here a detailed description of your App. What is it intended to be used for. Which steps of analyses are performed and how. Please be explicit about any detail that is important for use and understanding of the App and its outcomes.*

### Input data
*Indicate which type of input data the App requires. Currently only R objects of class `MoveStack` can be used. This will be extend in the future.*

*Example*: MoveStack in Movebank format

### Output data
*Indicate which type of output data the App produces to be passed on to subsequent apps. Currently only R objects of class `MoveStack` can be used. This will be extend in the future. In case the App does not pass on any data (e.g. a shiny visualization app), it can be also indicated here that no output is produced to be used in subsequent apps.*

*Example:* MoveStack in Movebank format

### Artefacts
*If the App creates artefacts (e.g. csv, pdf, jpeg, shapefiles, etc), please list them here and describe each.*

*Example:* `rest_overview.csv`: csv-file with Table of all rest site properties

### Parameters 
*Please list and define all parameters that the App requires to be set, if necessary including their unit.*

*Example:* `radius`: Defined radius the animal has to stay in for a given duration of time for it to be considered resting site. Unit: `metres`.

### Null or error handling
*Please indicate for each parameter as well as the input data which behaviour the App is supposed to show in case of errors or NULL values/input. Please also add notes of possible errors that can happen if parameters are improperly set and any other important information that you find the user should be aware of.*

*Example:* **Parameter `radius`:** If no radius AND no duration are given, the input data set is returned with a warning. If no radius is given (NULL), but a duration is defined then a default radius of 1000m = 1km is set. 

## R Library management
The template is prepared to use [`renv` as a dependency manager](https://rstudio.github.io/renv/articles/renv.html) - but is disabled ("opt-in") by default. You can [activate `renv` with `renv::activate()`](https://rstudio.github.io/renv/articles/renv.html#uninstalling-renv) and then use it in the [usual `renv` workflow](https://rstudio.github.io/renv/articles/renv.html#workflow).