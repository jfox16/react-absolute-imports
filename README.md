# Useful JS Stuff

## Prettier
`./.prettierrc.json`
```json
{
	"trailingComma": "none",
	"tabWidth": 2,
	"semi": false,
	"singleQuote": true
}

```

## Absolute Imports

`./jsconfig.json`
```json
{
  "compilerOptions": {
    "module": "commonjs",
    "target": "es2016",
    "jsx": "preserve",
    "checkJs": true,
    "baseUrl": "./src"
  },
  "exclude": ["node_modules", "**/node_modules/*"]
}
```

`./.env`
```
NODE_PATH=src/
```

## Testing in VSCode with Nodemon

Paste this into launch.json
```
{
    "version": "0.2.0",
    "configurations": [
        {
            "type": "node", 
            "request": "launch",
            "name": "nodemon",
            "runtimeExecutable": "nodemon",
            "program": "${workspaceFolder}/bin/www",
            "restart": true,
            "console": "integratedTerminal",
            "internalConsoleOptions": "neverOpen",
            "env": {
                "debug": "app:*",
            }
        }
    ]
}
```
