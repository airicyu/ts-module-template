# TypeScript nodejs(14.x.x) library starter

A template for very basic typescript nodejs module template with:
- basic project structure
- basic typescript config
- jest config for testing
- eslint integration
- prettier for code formatting

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