# Tips-NodeJS-y-TypeScript
Tips start project NodeJS with TypeScript


npm init -y = creacion rapida del package.json para proyecto

tsc --init = Crea archivo de configuracion de typescript

Instalacion de librerias para iniciar con TS en Node

yarn add typescript -DE

yarn add ts-node -DE  


ts-node src/index.ts -> Nos permite ejecutar archivos TypeScript

Agreganmos librerias de nuestra configuracion del proyecto: 
yarn add nodemon prettier eslint @typescript-eslint/eslint-plugin @typescript-eslint/parser -DE

Agregamos nuestro Framework Express

yarn add express

Agregamos nuestro script

"scripts": {
    "dev": "ts-node src/index.ts"
  },


con esta linea indicamos el archivo de entrada del proyecto:

"main": "index.ts",
