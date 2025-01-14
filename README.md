## Recommendation

**UPDATE 24.08**
the only rational solution for today is... [Vite](https://vitejs.dev/)

This project was created before the advent of the [Parcel](https://parceljs.org) tool. If you need a bundler for small and medium projects - I strongly suggest using Parcel instead. :)

## Webpack JS App - webpack 4 (4.29.6) JavaScript boilerplate

Generator pozwala za pomocą jednej komendy npm wygenerować boilerplate aplikacji
ze skonfigurowanymi środowiskami `dev, test(TBD), prod`.

Idealny boilerplate do tworzenia prostych stron oraz aplikacji webowych w czystym JS.
Narzędzie, pomimo iż z założenia przeznaczone głównie dla początkujących, może być śmiało wykorzystywane przez bardziej doświadczonych developerów, którzy nie mają czasu na ręczną konfigurację webpacka.

Aktualnie dostępny jest jeden config: **webpack-onepage-js-starter**, prace nad **webpack-spa-js-starter** in progress.

## Instalacja:

Node 11.10+

```
npm i -g webpack-js-app
webpack-js-app
> ? What project template would you like to generate?
> ? Project name: my-app

cd my-app
npm install
```

<p align="left">
  <img width="800" src="https://rawcdn.githack.com/czechue/webpack-js-app/807f597bc3c5050565f6fafe762f5cdef70ed357/demo.svg">
</p>

## Development

- `npm start` - startuje środowisko dev na: `http://localhost:8080`
- `npm run build` - buduje wersję produkcyjną

## Konfiguracje

### Porównanie

|                         | webpack-onepage-js-starter | webpack-spa-js-starter (TBD) |
| :---------------------- | :------------------------: | :--------------------: |
| Hot Module Replacement  |     :white_check_mark:     |   :white_check_mark:   |
| Dev Environment         |     webpack-dev-server     |   webpack-dev-server   |
| Basic prod minification |     :white_check_mark:     |   :white_check_mark:   |
| CSS Preprocessor        |        Sass (scss)         |      Sass (scss)       |
| CSS Modules             |            :x:             |   :white_check_mark:   |
| Autoprefixer            |     :white_check_mark:     |   :white_check_mark:   |
| Normalize.css           |     :white_check_mark:     |   :white_check_mark:   |
| Html template           |     :white_check_mark:     |          :x:           |
| Babel 7 compiled JS     |     :white_check_mark:     |   :white_check_mark:   |
| Unit Tests              |            :x:             |   :white_check_mark:   |
| E2E Tests               |            :x:             |   :white_check_mark:   |
| Eslint                  |            :x:             |   :white_check_mark:   |
| Prettier                |            :x:             |   :white_check_mark:   |

### Webpack-onepage-js-starter

- minimalistyczny, idealny do tworzenia stron typu one page,
- kod (strukturę) strony można w całości pisać zarówno w plikach index.html bądź javascript,
- w razie potrzeby config można bardzo prosto rozbudować o wszelkie funkcjonalności dostępne w webpack-spa-js-starter,

### Webpack-spa-js-starter (TBD)

- idealny do tworzenia aplikacji SPA,
- kod strony pisany w JS,
- skonfigurowane środowisko testowe,
- bardziej skupiony na web performance,

### Struktura katalogów

```
|-- package.json
|-- .editorconfig
|-- config
|-- dist
|-- src
|    |-- index.html
|    |-- scripts
|    |    |-- index.js
|    |
|    |-- styles
|    |    |-- main.scss
|    |    |-- base
|    |    |     |-- _base.scss
|    |    |     |-- _typography.scss
|    |
|    |-- assets
|

// webpack-spa-js-starter has also:

|-- __e2e__
|    |-- example.test.js
|
|-- src
|    |-- scripts
|    |    |-- index.js
|    |    |-- index.test.js
|
|-- .eslintrc.json
|-- .prettierrc
```

### Testy (TBD)

Webpack-spa-js-starter korzysta z następujących narzędzi:

- Jest https://github.com/facebook/jest
- DOM-Testing-Library https://github.com/kentcdodds/dom-testing-library
- Puppeteer https://github.com/GoogleChrome/puppeteer
- Jest-Pupeteer https://github.com/smooth-code/jest-puppeteer
- Pixelmatch https://github.com/mapbox/pixelmatch

## Przykłady (TBD)

Przykłady wykorzystania znajdują się w katalogu `/examples`
