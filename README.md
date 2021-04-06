# firebase-javascript
Realizar un deploy mediante el hosting de firebase para una página web base.

* Tener una cuenta en Firebase: https://firebase.google.com/
* Darle a comenzar.
* Agregar un proyecto.
* Agregar un nombre, será el dominio del sitio: fire-javascriptv1
* Se creará el repositorio y brindará pasos a seguir.
* Darle a Hosting y comenzar.

* Pasos dados por Firebase:
    * npm install -g firebase-tools
    * firebase login (Si ya se encuentra logueado, darle a logout para cambiar de cuenta)
    * firebase init
        * ? Are you ready to proceed? (Y/n) --> y
        * Elegir Hosting, bajar con flechas, seleccionar con la tecla espacio
        * Use an existing project --> porque se selecciona el proyecto antes creado (fire-javascriptv1)
        * ? What do you want to use as your public directory? (public) --> escribir un punto (.)
        * ? Configure as a single-page app (rewrite all urls to /index.html)? (y/N) --> y
        * ? Set up automatic builds and deploys with GitHub? (y/N) --> y
        * ? File ./index.html already exists. Overwrite? (y/N) -- n, porque ya se tiene el index
        * ? For which GitHub repository would you like to set up a GitHub workflow? (format: user/repository) --> se escribe el nombre del repositorio, junto con el usuario, chrisxavix/firebase-javascript
        * ? Set up the workflow to run a build script before every deploy? (y/N) --> y
        * ? What script should be run before every deploy? (npm ci && npm run build) --> darle doble enter
        * ? Set up automatic deployment to your site's live channel when a PR is merged? (Y/n) --> y
        * ? What is the name of the GitHub branch associated with your site's live channel? (master) --> darle a enter

* firebase deploy

* Nos arroja un enlace que será el proyecto desplegado: https://fire-javascriptv1.web.app

* Para futuros commits borrar: (- run: npm ci && npm run build) de los dos archivos de .github