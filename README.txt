# Creamos nuestra app next
npx create-next-app platzistore

# Lanzar servidor de desarrollo
npm run dev

# Una buena práctica es crear una carpeta llamada /src y mover a esta carpeta /pages, /styles y /public

-- En la raiz principal creamos el archivo: jsconfig.json
-- En la raiz principal creamos el archivo: .eslintignore
-- Renombramos el archivo .eslintrc.json a .eslintrc.js
-- En la raiz principal creamos el archivo: prettier.config.js

# Instalamos los siguientes paquetes
npm i prettier eslint-plugin-prettier eslint-plugin-jsx-a11y eslint-config-prettier eslint-config-next

# Instalamos paquete de sass
npm install sass

# Instalamos el paquete axios
npm install axios

Los archivos creados en la carpeta /pages next los va convertir en rutas, los archivos con un _name son ignorados, los va considerar como un archivo de configuración

# Para buscar errores en nuestra aplicación antes de enviarla a producción
npm run lint

# Agregamos en package.json
"scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "lint": "next lint",
    "lint:fix": "eslint src/ --fix"
},

# Para buscar reparar automáticamente ejecutamos
npm run lint:fix

# Para enviar a producción
npm run build

# Para lanzar en modo producción
npm run start