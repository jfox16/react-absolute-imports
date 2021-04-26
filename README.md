# Useful JS Stuff

## Absolute Imports
Create files called ```jsconfig.json``` and ```.env``` in your base directory, then copy-paste this code in.


In ```jsconfig.json```:
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

In ```.env```:
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
