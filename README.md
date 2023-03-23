<!-- GETTING STARTED -->

## Getting Started

### Prerequisites

- npm

  ```sh
  npm install -g npm@latest
  ```

  ```sh
  npm -v
  ```

 - Node

    ```sh
    sudo apt install -y curl
    ```

    ```sh
    curl -sL https://deb.nodesource.com/setup_19.x | sudo -E bash -
    ```

    ```sh
    sudo apt install -y nodejs
    ```

    ```sh
    node -v
    ```

### Create Vite Project

1. Vite installation

```sh
   npm create vite@latest
```
  
  ```sh
  npm install
  ```


2. Tailwind installation

- Terminal

```sh
npm install -D tailwindcss postcss autoprefixer
```

```sh
npx tailwindcss init -p
```

3. Tailwind config

- tailwind.config.js

```js
/** @type {import('tailwindcss').Config} */

module.exports = {
  content: ["./src/**/*.{js,jsx}"],
  theme: {
    extend: {
      screens: {
        xs: "400px",
        // => @media (min-width: 640px) { ... }

        sm: "640px",
        // => @media (min-width: 640px) { ... }

        md: "768px",
        // => @media (min-width: 768px) { ... }

        lg: "1024px",
        // => @media (min-width: 1024px) { ... }

        xl: "1280px",
        // => @media (min-width: 1280px) { ... }

        "2xl": "1536px",
        // => @media (min-width: 1536px) { ... }
      },
      fontFamily: {
        inter: ["Inter var", "sans-serif"],
      },
      boxShadow: {
        card: "0 0 1px 0 rgba(189,192,207,0.06),0 10px 16px -1px rgba(189,192,207,0.2)",
        cardhover:
          "0 0 1px 0 rgba(189,192,207,0.06),0 10px 16px -1px rgba(189,192,207,0.4)",
      },
    },
  },
  plugins: [],
};
```

- src/index.css

  ```css
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
  ```

3. Run

```sh
  npm run dev
```
