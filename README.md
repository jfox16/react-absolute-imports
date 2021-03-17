# react-absolute-imports
Some code to add absolute imports to react. Mostly for my own reference.


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
