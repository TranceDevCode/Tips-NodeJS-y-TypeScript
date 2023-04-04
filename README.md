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
    "dev": "ts-node src/index.ts",
    "format": "", Formatea el codigo
    "lint": "", 
    "lint:fix": ""  
  },


con esta linea indicamos el archivo de entrada del proyecto:

"main": "index.ts",

configurando el tsconfig.json:

{
  "compilerOptions": {
    "module": "CommonJS", /* Permite que mi codigo ts lo transpile al JS Nativo */
    "esModuleInterop": true, /* Permite tener compatibilidad con otras extensiones y modulos de otros lenguaje y del mismo entorno */    
    "resolveJsonModule": true, /* me permite darle soporte a impotar en mi codigo archivos json */
    "moduleResolution": "node", /* permite reconocer o darle soporte absoluto a typescript al compilar */
    "target": "ES2020", /* Me pertime especificar la estandarizacion del EcmaScript para mi proyecto*/
    "noImplicitAny": true, /* Me permite definir que no me recomiende tipar con tipos any por default */
    "sourceMap": true, /* Me permite crear un archivo js raiz identificador para cada archivo generado a partir de ts, se genera con el comando tsc */
    "experimentalDecorators": true, /* me permite darle soporte a mi proyecto para trabajar con decoradores */
    "emitDecoratorMetadata": true, /* Me permite que la data que generen los decoradores persistan en tiempo de ejecucion */
    "strict": true, /* Me permite identificar algunas definiciones de errores para tu codigo  */
    "baseUrl": "./", /* Me permite definir donde alojare mi directorio que tiene el codigo para produccion */
    "outDir": "./build" /* Este es el directorio con mi codigo js para produccion */
  },
  "exclude": ["node_modules"], /* Me permite ignorar el directorio de node module*/
  "include": ["src/**/*.ts"],  /* me permite definir donde se va a encontrrar mi codigo a compilar/transpilar */
}

