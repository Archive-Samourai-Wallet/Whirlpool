# Whirlpool architecture


## I. Usage
Whirlpool can be managed:
- from desktop: `whirlpool-gui`
- from REST API for developers: `whirlpool-cli API`
- from command line: `whirlpool-cli`

![](charts/usage.png)


## II. Modules
Whirlpool is modular:
- 4 java modules: `server`, `client`, `protocol`, `cli`
- 1 electron/react module: `GUI`

`client` and `server` communicate through `protocol`.

![](charts/architecture.png)

