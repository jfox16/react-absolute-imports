# How to add absolute imports to React
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

in ```.env```:
```
NODE_PATH=src/
```
