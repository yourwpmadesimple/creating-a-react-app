# Getting Started with Create React App

## Create React APP
### Create a react js project.
```
npx create-react-app <project_name>
```
## Installing dependencies
### Installing react icons.
```
npm install react-icons --save
```

### Installing tailwind css.
```
npm install -D tailwindcss@npm:@tailwindcss/postcss7-compat @tailwindcss/postcss7-compat 
postcss@^7 autoprefixer@^9 @tailwindcss/forms --force
```

### Creating tailwind config file
```
npx tailwindcss init
```
#### tailwind.config.js
```
module.exports = {
    purge: ['./src/**/*.{js,jsx,ts,tsx}', './public/index.html'],
    darkMode: false, // or 'media' or 'class'
    theme: {
        extend: {},
    },
    variants: {
        extend: {},
    },
    plugins: [require('@tailwindcss/forms')]
}
```

### Installing Craco
```
npm install @craco/craco --legacy-peer-deps (or ---force)
```

#### pacakage.json
In your package.json file replace react-scripts with craco
```
ORIGINAL
"scripts": {
        "start": "react-scripts start",
        "build": "react-scripts build",
        "test": "react-scripts test",
        "eject": "react-scripts eject"
    },
```
```WITH CRACO REPLACEMENT
"scripts": {
        "start": "craco start",
        "build": "craco build",
        "test": "craco test",
        "eject": "react-scripts eject"
    },
```
```
