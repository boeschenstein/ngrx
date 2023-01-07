# NgRx

<https://ngrx.io/>

## Learn

<https://app.pluralsight.com/library/courses/angular-ngrx-getting-started>

## Container + Presentation 

(smart/dumb, fat/skinny, stateful/pure, components/screens)

- Konzept: https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0
- Rainer Hahnekamp: https://www.rainerhahnekamp.com/en/ngrx-best-practices-series-2-modularity/

Container                                               | Presentation 
--:                                                     | :--
Concerned with how things work                          | Concerned with how thinks look
Have little or no HTML and CSS styles                   | HTML markup and CSS styles
Have injected dependencies                              | No dependencies on the rest of the app
Are stateful and specify how data is loaded and changed | Don't specify hwo data is loaded or changed but emit events via @Output
Top level routes                                        | Receive data via @Inputs
May contain other components                            | May contain other components
