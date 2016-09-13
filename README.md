# omastar

Aplicación con el objetivo de armar la arquitectura y elegir las librerias a usar en Olpays

![Omastar](http://vignette1.wikia.nocookie.net/pokemon/images/6/65/Omastar_IL046.png/revision/latest?cb=20150624040620)

## [Styling](http://stackoverflow.com/questions/26882177/react-js-inline-style-best-practices)

* CSS
* Inline CSS

## Herramientas styling

* CSS: Less, Sass, import CSS in components
* Inline: Radium, ...
* CSS Modules

## Testing
* [Testing strategies](https://github.com/facebookincubator/create-react-app/blob/master/template/README.md#testing-components)
  * Smoke tests provide the biggest value with the least effort. A smoke test verifies a component renders without throwing
  * Test parts of a component that are worth testing. A good rule used to determine whether a component needs testing is: when a change in a component introduces bugs, it might be a good time to introduce tests asserting specific behaviour
  * [Jest snapshot tests](https://facebook.github.io/jest/blog/2016/07/27/jest-14.html) let you make sure your component did not change unexpectedly. This lets you spend less time writing tests and more time writing components
  * Snapshot tests work great for component testing that tests component behaviour by injecting custom props and state
  * Enzyme works great for end-to-end style tests that simulate user actions
* [Comparison between snapshot tests and enzyme](https://blog.callstack.io/unit-testing-react-native-with-the-new-jest-i-snapshots-come-into-play-68ba19b1b9fe#.3l5ss330w)

## State management

* Redux
  * Cuando usar redux y cuando manejar estado en componente?
  * Time traveling?
  * Convenciones de acciones. Ejemplo: https://github.com/acdlite/flux-standard-action

## Translations

## Immutable o no?

## UI Framework
 * Material UI
 * React Native web o no?
 * [React toolbox](http://react-toolbox.com/#/) usa css modules

## Componentes
 * Que tan reusable hacer nuestros componentes? Hagamos componentes agnosticos al framework de UI que usen. Esto nos llevaria a componentes reutilizables en web/mobile, codigo mas reutilizable y a la larga quizas cambiar de framework UI
   * Separar entre [componentes de presentacion y componentes contenedores](https://medium.com/@dan_abramov/smart-and-dumb-components-7ca2f9a7c7d0#.37cfpqa29). Con esto logramos reutilizar por completo los componentes contenedores en web/mobile.
   * Diseñar componentes de manera que tengan dos capas de abstracción. La capa superior sólo puede utilizar otros componentes de la aplicación, NO puede utilizar elements específicos de la plataforma (ej. no utilizar `div`, `span` o `li`). La capa inferior es la implementación del componente en la plataforma, por lo tanto esta sí puede usar `div`s, `span`s y `li`s
 * Utilizar variables en las propiedades de los componentes. Ejemplo: <Button onClick={() => createStuff()} /> en vez de <Button onClick={() => foo.isBar ? foo.map(fo => fo.doSomething() : this.setState({ foo: null }))} />

## ES6 classes o React.createClass?

## Routing

* React router?
* Hay alguna otra opción? [Al parecer no se lleva muy bien con redux](https://formidable.com/blog/2016/07/11/let-the-url-do-the-talking-part-1-the-pain-of-react-router-in-redux/)
  * Si hay otra opcion! [Redux little router](https://github.com/FormidableLabs/redux-little-router)

## Types

* Flow
* Typescript
* Js

## Animaciones

## Libreria graficos

## Formularios

## Icon system

## Naming and directory structure conventions
* http://marmelab.com/blog/2015/12/17/react-directory-structure.html
* http://jaysoo.ca/2016/02/28/organizing-redux-application/

## Server rendering

# Look and feel
