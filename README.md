# @ontario-digital-service/prettier-config-ontario

This package provides the [html-validate](https://html-validate.org) configuration adhering to the Ontario Frontend JavaScript validation guide, which will be released in the future. This configuration aims to validate the markup in Ontario Frontend projects.

## Rules & Exceptions

- **Void Style**: the linter will not enforce any particular style for void elements such as `<img>`, `<br>`, `<input>`, etc.

- **Prefer Button**: allowing the use of `<input type="button">`.

- **SVG Focusable**: not checking svg elements for the `focusable` attribute.

- **Trailing Whitespace**: allowing the output html in `dist` folder to have whitespaces, that could occur due to the merging of several templates into HTML.

## Installation

To integrate the Ontario html-validate configuration into your project, choose one of the following methods based on your package manager:

### NPM

1. First, you need to install [HTML-validate](https://html-validate.org)if it's not already installed:

```sh
npm install html-validate --save-dev
```

2. Next, install the `@ontario-digital-service/html-validate-ontario` package:

```sh
npm install @ontario-digital-service/html-validate-ontario --save-dev
```

### YARN

```sh
yarn add @ontario-digital-service/html-validate-ontario --dev
```

## Usage

### Basic Usage

Run the following:

```json
"html-validate-ontario"
```

### Customizing Configuration

For projects that require customization beyond the base configuration, you can extend and override specific settings. Create a `.htmlvalidate.js` file in your project's root directory, import the Ontario configuration, and then add your modifications:

```javascript
module.exports = {
  ...require('@ontario-digital-service/html-validate-ontario')
  };
```

This approach allows you to maintain the foundational style guide while tweaking aspects that are project-specific or according to your team's preferences.

## Contributing

We welcome contributions to improve the prettier-config-ontario package. Please feel free to submit a pull request or open an issue on our [GitHub repository](https://github.com/syed-ods/html-validate-ontario).