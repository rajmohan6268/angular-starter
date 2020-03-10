# <center> Angular-Tailwind-ESLint </center>

A remake of the default starter app project generated by [Angular CLI](https://github.com/angular/angular-cli) (version 9.0.4).


## Overview

### Angular

To improve readability, I have leveraged structural directives where possible. This of course means the app is now a little more dependent on JavaScript.

### Tailwind CSS
The original code has been modified to use [Tailwind CSS](https://tailwindcss.com/). I have employed its utility classes as much as possible to give the app a similar look and feel to the original, including various effects and animations.

For more information on how to integrate the two frameworks, please read the excellent [Angular 8/9 + Tailwind CSS Guide](https://dev.to/seankerwin/angular-8-tailwind-css-guide-3m45) written by Sean Kerwin at [DEV](https://dev.to/).

### Inline SVGs

To reduce clutter, I have moved inline `<svg/>` tags to their own file in the assets folder. These are now dynamically loaded by the [ng-inline-svg](https://github.com/arkon/ng-inline-svg) package, using a minimal custom component.

### ESLint

Linting is configured to use [ESLint](https://eslint.org/) with the [angular-eslint](https://github.com/angular-eslint/angular-eslint) project. I followed the configuration examples referenced in their repository and it pretty much _just works&trade;_. Kudos to the team for the fantastic job they are doing.


## Development

The application was installed using [pnpm](). The `pnpm-lock.yaml` shrinkwrap file is provided.

#### Angular

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

#### Scripts

```sh
pnpm run start      # start development server
pnpm run lint       # lint files using angular-eslint
pnpm run build      # build the project to /dist
pnpm run test:e2e   # run end-to-end tests via Protractor
pnpm run test:unit  # run unit tests via Karma
```
