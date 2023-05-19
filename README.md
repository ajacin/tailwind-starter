# Installing tailwind CLI

Follow

> npm i -D tailwindcss

- -D only as dev dependency
  npx tailwindcss init

# Instead of build process

```
"scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "build": "tailwindcss -i ./input.css -o ./css/style.css",
    "watch": "tailwindcss -i ./input.css -o ./css/style.css --watch"
  },
```

npm run build should create a css folder and styles.css file

npm run watch to watch
