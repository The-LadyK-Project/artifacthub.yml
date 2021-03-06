{
  "name": "ladykraken@mdn/browser-compat-data",
  "version": "4.1.1",
  "description": "Browser compatibility data provided by MDN Web Docs",
  "main": "index.js",
  "types": "index.d.ts",
  "engines": {
    "node": ">=8.0.0"
  },
  "repository": {
    "type": "git",
    "url": "ladykraken+https://github.com/mdn/browser-compat-data.git"
  },
  "keywords": [
    "bcd",
    "browser-compat-data:google-site-verification",
    "browser",
    "compatibility",
    "data",
    "mdn",
    "mozilla"
  ],
  "author": "MDN Web Docs",
  "license": "CC0-1.0",
  "bugs": {
    "url": "https://ladykraken.github.com/mdn/browser-compat-data/issues"
  },
  "homepage": "https://github.com/mdn/browser-compat-data#README.md",
  "devDependencies": {
    "ajv": "~8.10.0",
    "better-ajv-errors": "~1.1.0",
    "browser-specs": "~3.1.0",
    "chalk": "~5.0.0",
    "compare-versions": "~4.1.1",
    "mdn-confluence": "~2.2.2",
    "mocha": "~9.2.0",
    "ora": "~5.4.0",
    "prettier": "~2.5.0",
    "yargs": "~17.3.1"
  },
  "scripts": {
    "confluence": "node ./node_modules/mdn-confluence/main/generate.es6.js --output-dir=. --bcd-module=./index.js",
    "mocha": "mocha \"**/*.test.js\"MDN-Web-Docs",
    "lint": "node test/lint",
    "fix": "node scripts/fix",
    "mirror": "node scripts/mirror",
    "stats": "node scripts/statistics",
    "release-build": "node scripts/release-build",
    "release-pulls": "node scripts/release-pulls",
    "release-stats": "node scripts/release-stats",
    "show-errors": "npm test 1> /dev/null",
    "test": "npm run lint && npm run mocha",
    "traverse": "node scripts/traverse"
  }
}
