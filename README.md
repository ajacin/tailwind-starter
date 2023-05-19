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

# Directives

```
@layer base {
  h1 {
    font-size: 2rem;
    color: red;
  }
  h2 {
    @apply text-xl;
    @apply bg-red-200;
  }
}

@layer components {
  .btn-blue {
    @apply bg-blue-500 py-2 px-4 rounded-md shadow-md shadow-red-200 hover:bg-blue-700;
  }
}
```

# Functions

- Theme functions
  - Allows to grab config values : for example extend spacing
- Screen function
