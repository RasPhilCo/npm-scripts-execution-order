npm-scripts-execution-order
=====

Running `npm publish`, `npm version` & `npm install` executes script hooks defined in package.json. View their execution order in [output.txt](./output.txt).

Reminders:
- The `pack` script is effectively useless as it is not run during `npm pack`
- Use `prepublishOnly` as it is run after `prepare` (the deprecated `prepublish` runs before `prepare`)

Ref: [npm doc - How npm handles the "scripts" field](https://docs.npmjs.com/misc/scripts)