# TypeScript nodejs(14.x.x) library starter

A template for very basic typescript nodejs module template with:
- basic project structure
- basic typescript config
- jest config for testing
- eslint integration
- prettier for code formatting

---

## project strcture

### source root
./src

### type root dir
./src/types

### test root
./test

### compile output
./dist/lib

### compile types
./dist/types

---

## commands

build: `npm run build`

watch build: `npm run watch`

test: `npm test`

watch test: `npm run test:watch`

format code: `npm run format`

lint: `npm run lint`

---

## VS code debug launch config

```json
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "node",
            "request": "launch",
            "name": "Launch Program",
            "program": "${workspaceFolder}\\dist\\lib\\src\\main.js",
            "preLaunchTask": "tsc: build - tsconfig.json",
            "outputCapture": "std",
            "skipFiles": [
                "<node_internals>/**",
                "${workspaceFolder}/node_modules/**/*.js"
            ],
            "outFiles": [
                "${workspaceFolder}/dist/lib/**/*.js"
            ]
        }
    ]
}
```