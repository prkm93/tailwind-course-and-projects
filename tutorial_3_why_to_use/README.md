# Why to use Tailwind CSS ?

- No reinventing of CSS class names required - ex - we need to thnk and add class names everytime when need to add new stlyes to div
- Your CSS doesn't grow with html and designs - utility classes make components independent. ex - styles of navbar of one page, willn't collapse with styles of navbar of other page.

- When you make a change, no risk of breaking existing templates

- Will it make site slow ? Will it increase bundle size ? -> No

# How to setup tailwind css ?

- `npm init -y` // initializes directory as node project
- `npm install -D tailwindcss postcss autoprefixer vite` // installs required packages
- `npx tailwindcss init -p`
- Create CSS file "main.css". Add it to HTML and edit it with content.
  ```
     @tailwind base;
     @tailwind components;
     @tailwind utilities;
  ```
- In `tailwind.config.js` file, replace **_content : []_** with **_content : ["*"]_**
- Add `"start:"vite"` to `package.json`
