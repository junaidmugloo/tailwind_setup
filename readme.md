# make 2 folders one is dict and another src
# make index file under dict folder
# make input.css file under src folder
# add three lines code in input.css
# @tailwind base;
# @tailwind components;
# @tailwind utilities;
# open terminal and hit command npx tailwindcss init 
# open tailwind.config.js 
# and add this code
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./dist/**/*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}

# hit this command to compile css 
# npx tailwindcss -i ./src/input.css -o ./src/output.css --watch
# it give output file now link this output.css file into you html 

