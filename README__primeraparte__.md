El único requisito es que tengas Node.js instalado en tu computador.
En tu terminal, ve a la carpeta que contiene tu proyecto y pega estos dos comandos:

Paso 1: Ejecuta npm init -y

Paso 2: Ejecuta npm install babel-cli@6 babel-preset-react-app@3

Aquí sólo estamos usando npm para instalar el preprocesador de JSX; no lo vas a necesitar para nada más. Tanto React como el código de la aplicación pueden seguir como una etiqueta de <script> sin cambio alguno.
Ejecuta el preprocesador de JSX
Crea una carpeta llamada src y ejecuta este comando en la terminal:

npx babel --watch src --out-dir . --presets react-app/prod

No esperes hasta que termine — este comando inicia un observador automático para JSX.
Si ves algún mensaje de error que te dice que “Has instalado equivocadamente el paquete de babel”, puede ser que olvidaste realizar el paso anterior. Realiza el paso anterior en la misma carpeta en que estás y vuelve a intentar este paso.
si ahora creas un archivo llamado src/like_button.js con este codigo incial, el observador va a crear un like_button.js preprocesado con el código JavaScript original que es apto para el navegador.
por ultimo debes crear el archivo .gitignore y dentro escribes node_modules Esto ignorará todos los archivos que  se encuentren en la carpeta node_modules
tambien puedes usar 
*.dat
resultados/
ignorarArchivo.txt
Esto ignorará todos los archivos que terminen en .dat, todos los archivos que se encuentren en la carpeta resultados, e ignorará el archivo ignorarArchivo.txt