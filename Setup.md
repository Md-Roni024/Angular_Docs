### Setup New Project in Angular
Create New Project
```bash
ng new project_name
```

Serve Application
```bash
cd project_name
ng serve --open
```
Run the command to create a Component, inside src/app.
```bash
ng generate component components/Header
ng generate component components/Footer
ng generate component components/Main
```

Run the Command to create a Service
```bash
ng generate service services/Product
ng generate service services/Customer
```




### Setup Tailwind in Angular Project
Initial Command
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init
```

Go to tailwind.config.js and paste this in content
```bash
  content: [
    "./src/**/*.{html,ts}",
  ],
```

Go to style.css and paste this
```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

