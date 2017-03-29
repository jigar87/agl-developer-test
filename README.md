# AGL Developer Programming Challenge

This is a sample code to consume a json hosted at [ http://agl-developer-test.azurewebsites.net/people.json]( http://agl-developer-test.azurewebsites.net/people.json) and output a list of all the cats in alphabetical order under a heading of the gender of their owner.

Example:

```yml
Male
- Angel
- Molly
- Tigger

Female
- Gizmo
- Jasper

```

## Scripts

```bash
# to install node modules (to be done once)
npm install

# to run the project
npm start

# to run test suites
npm test

# to create build
npm run build

# to run test cases in watch mode
npm run tdd
```

## Tools used

This project is written using the following tools:

- JavaScript [`ES2015`](https://babeljs.io/learn-es2015/) version
- [`Webpack 2.x`](https://webpack.js.org/) as module bundler
- [`Babel JS`](https://babeljs.io/) as the compiler.
- [`Mocha JS`](https://mochajs.org/) testing framework.
- [`Chai JS`](http://chaijs.com/) as the assertion library
- [`Istanbul JS`](https://istanbul.js.org/) as the code coverage library

## Output

![Coverage Report](./docs/output.png)

## Coverage

To get coverage report

```bash
npm test
```

![Coverage Report](./docs/coverage-report.png)

HTML Report can be accessed from [here](./coverage/index.html)

## Known Issue

The server does not support Cross Origin Resource Sharing (CORS), therefore the below error may be shown:

```bash
FAILED: Failed to fetch
```

To fix this, start Google Chrome with disabled web-security using the following command:

### In MAC
```bash
open -a "Google Chrome" --args --user-data-dir --disable-web-security
```

### In Windows
```bash
"C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --disable-web-security --user-data-dir="C:\chrome"
```