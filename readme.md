# Install Tailwind CSS

```sh
npm install -D tailwindcss
npx tailwindcss init
```


## Configure your template paths

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./html/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```


## Add the Tailwind directives to your CSS

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```


## Start the Tailwind CLI build process

```sh
npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
```

## Start using Tailwind in your HTML


```html
<!doctype html>
<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link href="./src/output.css" rel="stylesheet">
</head>
<body>
  <h1 class="text-3xl font-bold underline bg-yellow-200 text-center">
    Hello world!
  </h1>
</body>
</html>
```
