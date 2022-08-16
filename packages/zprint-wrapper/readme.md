# zprint wrapper

A [clojure zprint](https://github.com/kkinnear/zprint) wrapper published to npm with stdin/stdout support.

## Installation

Run the following command or add it as a dep to a node project:

```sh
npm install -g zprint-wrapper
```

## Usage

```sh
zprint --help
```

This wrapper also supports processing clojure code via stdin and printing to stdout.

```sh
echo "(fn [] (+ 1 2))" | zprint
```

## Development

Run `yarn dev` or `npm run dev` to start a repl and watcher for incremental builds.

Run the following to install the package locally with a symlink:

```sh
cd package
npm link
```

### Build script

Run `yarn build` or `npm build` to compile to package/main.js

Then try the following to update:

```sh
cd package
npm patch
npm publish
```

## Credits

Credit goes to https://github.com/thheller/zprint-npm for coming up with a
recipe to package up zprint and make it convenient to install with node.
