# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

node.js installed
npx create-react-app [ my-app ]
cd [ my-app ]
npm start

(bootswatch website for css file)
frontend: npm install react-bootstrap 

cdnjs.com  font awesome for icons

frontend: npm install react-router-dom react-router-bootstrap

if problem with importing [{} from'react-router-dom'] frontend:npm i --save-dev @types/react-router-dom --force 
react router instructor using is 5.2.0 Routing does not work so have to change syntax or downgrade router versions.

Django
global  pip install virtualenv
global virtualenv [myenv]
global myenv\scripts\activate  -doesnt work (powershell try powershell -ExecutionPolicy Bypass my\scripts\activate)
  (then click view>command pallete> type python:select interpreter. select global non-env)
pip list
pip install django
django-admin startproject [backend]
backend: python manage.py runserver
backend: [optional] python manage.py migrate(warning popped up on mine but not instructors)
backend: python manage.py startapp base

add 'base.apps.BaseConfig', to settings.py file (under installed apps)

backend: python manage.py runserver (to run the server)

backend: pip install djangorestframework
add 'rest_framework', to settings.py file

 section 3.13
frontend: npm install axios

backend: pip install django-cors-headers

add 'corsheaders', to settings.py file
add 'corsheaders.middleware.CorsMiddleware', to settings.py file (under middleware)
add CORS_ALLOW_ALL_ORIGINS = True to settings.py file 
frontend package.json add "proxy": "http://127.0.0.1:8000", (so don't have to include it at beginning of front end fetch request)

ProductScreen has second useParam issue end 3.13
3.14
backend: python manage.py migrate
backend: python manage.py createsuperuser  (will be prompted to enter username, email password. Enter fake) duane, duane@email, duane
jdango admin panel locahlhost:8000/admin/
3.15
backend: python manage.py makemigrations
backend: python manage.py migrate
 3.16
backend: pip install pillow (to be able to add image field to model.py. Will prompt you.)Then run 2 commands for migration

3.17

add MEDIA_URL = '/images/'  and STATICFILES_DIRS = [
    BASE_DIR / 'static'] and MEDIA_ROOT = BASE_DIR / 'static/images', to settings.py file

3.20
add Redux DevTools Chrome extension
fronend: npm install redux react-redux redux-thunk redux-devtools-extension
frontend : npm install @reduxjs/toolkit (if giving error) look at QA for help