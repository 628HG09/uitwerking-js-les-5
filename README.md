#Project Setup

###Stappenplan:
1. Create a new file named `.gitignore` and add the file paths that need to be ignored: 
```
/.idea
/.parcel-cache
/node_modules
```
2. Create a first commit
```
git init
git add .
git commit -m 'commit name here'
```
3. Create a new repository
```
git remote add origin git@github.com:your-git-username-here/project-name-here.git
git branch -M main
git push -u origin main
```

4. Create a feature branch
```
git checkout -b feature/feature-branch-name-here
```

5. Create new root folder named `src` and add `index.html`, `main.js` and `style.css` to the folder


6. Link the JS and CSS file to the HTML file (don't forget to set the _type_ attribute)
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="./style.css">
    <title>Title</title>
</head>
<body>

<script src="main.js" type="module"></script>
</body>
</html>
```

7. Initialization of Node Package Manager (and _enter_ through the basic setup):
```
npm init
```

8. Install developer _bundler_ package **Parcel**
```
npm install parcel --save-dev
```
9. Add _start_ command to  _srcipts_ object in the package.json file in order to run parcel
```
"scripts": {
   "start" : "parcel src/index.html",
},
```

10. Run your project
```
npm run start
```