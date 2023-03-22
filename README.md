# start-vite-project

Node & npm upgrade

(1). VITE
npm create vite@latest

(2). TAILWIND CSS
a. Terminal
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init

b. tailwind.config.js

---

---

/\*_ @type {import('tailwindcss').Config} _/

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

---

---

c. src/index.css
@tailwind base;
@tailwind components;
@tailwind utilities;

(3) npm run dev
