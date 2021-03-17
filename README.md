# How to add absolute imports to React
Create ```jsconfig.json``` and ``.env``` in your base directory, and copy-paste this code in.


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
