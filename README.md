# tailwindcss set up instruction 
Step 1: project set up as npm 
```
npm init -y
```
Step 2: install tailwindcss
```
npm install -D tailwindcss
```
Step 3: initialized tailwindcss
```
npx tailwindcss init
```
Step 4: add this <b>"*html"</b> in tailwind.config.js file

Step 5: Create file input.css in css folder
```
css\input.css
```
Step 6: add below code in input.css file
```
@tailwind base;
@tailwind components;
@tailwind utilities;
```
Step 7: make a scripts as build in package.json file (rename css insted of src)
```
"build":"npx tailwindcss -i ./css/input.css -o ./css/output.css --watch"
```

Step 8: downlaod tailwindcss extension
```
Tailwind CSS IntelliSense
```

Step 9: add link in html file (stylesheet) 
```
<link rel="stylesheet" href="./css/output.css"
```

Step 10: run build command in terminal to show output as live server
```
npm run build
```