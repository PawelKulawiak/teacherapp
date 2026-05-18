# teacherapp
## CCBES Teacher Report

A Quarto Shiny application that visualizes student well-being data based
on the *Perceptions of Inclusion Questionnaire* (PIQ; Venetz et al., 2015).

The app reads response data from a Google Sheet and computes three PIQ
scale scores per measurement occasion: *emotional*, *sozial*, and
*akademisch* well-being. Results are displayed as:

- interactive bar charts (`ggiraph`) showing the development of each
  dimension across weeks
- radar charts (`ggradar`), one per measurement occasion, to inspect
  the multivariate profile
- an AI-assisted interpretation chatbot (`shinychat` + `ellmer`,
  powered by the OpenAI API) that helps teachers interpret the patterns

## Tech stack

R, Quarto Shiny, `tidyverse`, `ggplot2`, `patchwork`, `ggiraph`,
`ggradar`, `bslib`, `googlesheets4`, `shinychat`, `ellmer`.

## Deployment

Deployed on shinyapps.io. Requires `OPENAI_API_KEY` in `.Renviron`.

## Reference

Venetz, M., Zurbriggen, C. L. A., Eckhart, M., Schwab, S., & Hessels,
M. G. P. (2015). *The Perceptions of Inclusion Questionnaire (PIQ)*.
https://piqinfo.ch/

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)
