# NgRx

<https://ngrx.io/>

## Learn

<https://app.pluralsight.com/library/courses/angular-ngrx-getting-started>

## Actions

### Action hygiene

Action hygiene is important: <https://www.youtube.com/watch?v=JmnsEvoy-gY>

> Do not reuse actions for different scenarios

```js
[Source] Event
```

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

## Search/Filter

### All data is client side: no no effect involved

> There is no need for rxjs, using this approach

1. add filter-property to state
2. use selector to filter data, using fiter-property (from state)
3. on input change, push fiter-property to state

### Using effect to filter on server side

<https://medium.com/front-end-weekly/managing-state-in-angular-apps-with-ngrx-store-and-ngrx-effects-part-3-99fe2e0a7082>

## Information

### Best practice

- https://indepth.dev/posts/1442/ngrx-bad-practices
