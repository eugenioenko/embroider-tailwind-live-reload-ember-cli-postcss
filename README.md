# embroider-tailwindcss-live-reload-purgecss

This repository is a minimal reproduction of ember app with embroider and tailwindcss using ember-cli-postcss. 
It contains an issue with live-reload for css not working


**Repro steps**
- start dev environment `npm run start`
- ones the app loaded modify `/app/templates/application.hbs` to inlcude new tailwind utility class
- wait for app to reload in the browser
**Expected**
- The new added utility classes are applied
**Observed**
- The new utility classes are not applied and an app restart is requried

**Notes**
postcssOptions do include `*.hbs` in the case
https://github.com/eugenioenko/embroider-tailwind-live-reload-ember-cli-postcss/blob/676739a1e0dc1e47e56cdcc9f14b055bc9a6481d/ember-cli-build.js#L10

## Prerequisites

You will need the following things properly installed on your computer.

- [Git](https://git-scm.com/)
- [Node.js](https://nodejs.org/) (with npm)
- [Ember CLI](https://cli.emberjs.com/release/)
- [Google Chrome](https://google.com/chrome/)

## Installation

- `git clone <repository-url>` this repository
- `cd embroider-tailwindcss-live-reload-purgecss`
- `npm install`

## Running / Development

- `npm run start`
- Visit your app at [http://localhost:4200](http://localhost:4200).
- Visit your tests at [http://localhost:4200/tests](http://localhost:4200/tests).

### Code Generators

Make use of the many generators for code, try `ember help generate` for more details

### Running Tests

- `npm run test`
- `npm run test:ember -- --server`

### Linting

- `npm run lint`
- `npm run lint:fix`

### Building

- `npm exec ember build` (development)
- `npm run build` (production)

### Deploying

Specify what it takes to deploy your app.

## Further Reading / Useful Links

- [ember.js](https://emberjs.com/)
- [ember-cli](https://cli.emberjs.com/release/)
- Development Browser Extensions
  - [ember inspector for chrome](https://chrome.google.com/webstore/detail/ember-inspector/bmdblncegkenkacieihfhpjfppoconhi)
  - [ember inspector for firefox](https://addons.mozilla.org/en-US/firefox/addon/ember-inspector/)
