# Project Setup

1. Create two folders: `dist` and `src`.

2. Inside the `dist` folder, create an `index.html` file.

3. Inside the `src` folder, create an `input.css` file with the following content:

    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

4. Open your terminal and run the following command to initialize Tailwind CSS:

    ```bash
    npx tailwindcss init
    ```

5. Open the generated `tailwind.config.js` file and replace its content with the following code:

    ```js
    /** @type {import('tailwindcss').Config} */
    module.exports = {
      content: ["./dist/**/*.{html,js}"],
      theme: {
        extend: {},
      },
      plugins: [],
    }
    ```

6. Compile the CSS by running the following command:

    ```bash
    npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
    ```

7. Link the generated `output.css` file to your `index.html` file inside the `dist` folder.

Your project structure should look like this:

    ```plaintext
    project-root
    ├── dist
    │   └── index.html
    ├── src
    │   └── input.css
    ├── tailwind.config.js
    └── package.json (after running `npm init` and installing tailwindcss)
    ```
