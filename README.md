# react-absolute-imports
Some code to add absolute imports to react. Mostly for my own reference.


```jsconfig.json```
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

```.env```
```
NODE_PATH=src/
```
