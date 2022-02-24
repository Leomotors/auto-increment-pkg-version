# @leomotors/automation

[![](https://img.shields.io/npm/v/@leomotors/automation.svg?maxAge=3600)](https://www.npmjs.com/package/@leomotors/automation)
[![](https://img.shields.io/npm/dt/@leomotors/automation.svg?maxAge=3600)](https://www.npmjs.com/package/@leomotors/automation)

_Most of the download probably come from me, 😂_

As its name suggests, it's a piece of code that I used a lot, so I decided to put it in npm then I can access it easily.

You are free to use this if you want the same thing as mine.

Please keep in mind that breaking change can be made at any point.

Here is some info in case you wonder what I'm doing.

## Scripts

_One you install this package, these scripts will be installed to `node_modules/.bin`_

lm-inc: Increment Patch Number by 1 when called

lm-config: Put some metadata into specified file (Default: src/config.ts)

```
lm-config {file name} {time zone (Default: Asia/Bangkok)}
```

- Parameter: File Path, in case you want to override default

### configPackage.js Output

```ts
export const Version = "3.0.0";
export const BuildTime = "2022-01-24 17:06:58";
```

## Example Usage in package.json

```json
"scripts": {
    "dev": "lm-inc && lm-config && smth dev",
    "build": "lm-config && smth build",
}
```
