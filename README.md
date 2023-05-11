# Pronovo Mail Templates

## Getting Started

Clone or download this repository. Then navigate into the directory and install dependencies:

```
npm install
```

Start local development:

```
npm run dev
```

Build emails for production:

```
npm run build
```

## Structure
These templates are built using Maizzle, a framework that helps you quickly build HTML emails with Tailwind CSS and advanced, email-specific post-processing.

### Templates
The templates are showcasing how the components can be used to build messages. All templates are based on the main layout provided and consist out of the maincomponents provided. 
- example-complete.html -> Showcases all available components and variants.
- example-simple.html -> Shows a simple message including a call to action.

### Components
Within the components directory are the building blocks for the templates. There are a number of handy components available to build your templates. 

- Button 
  -> add the attribute 'type="secondary"' to create a different type of button
- Content
- Divider
- Keyvisual
- Link
- Paragraph
- Spacer

Some of the components are used to build the main structure of the templates.
- Header
- Title
- Container
- Footer


## Build
All templates are output to the 'build_production' directory.
To build emails for production run:

```
npm run build
```

Maizzle refers to the settings in 'config.js'. These settings determine how the mails are built.
For example, the baseURL should be updated to link to the correct images on the Pronovo infrastructure.

```
baseURL: {
    url: 'http://pronovo.redefine.studio/',
    tags: ['img'],
  },
```


## Documentation

Maizzle documentation is available at https://maizzle.com

## License

The Maizzle framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

[npm]: https://www.npmjs.com/package/@maizzle/framework
[npm-stats]: https://npm-stat.com/charts.html?package=%40maizzle%2Fframework&from=2019-03-27
[npm-version-shield]: https://img.shields.io/npm/v/@maizzle/framework.svg
[npm-stats-shield]: https://img.shields.io/npm/dt/@maizzle/framework.svg?color=6875f5
[github-ci]: https://github.com/maizzle/framework/actions
[github-ci-shield]: https://github.com/maizzle/framework/actions/workflows/nodejs.yml/badge.svg
[license]: ./LICENSE
[license-shield]: https://img.shields.io/npm/l/@maizzle/framework.svg?color=0e9f6e
