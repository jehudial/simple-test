# Simple-test

This This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.
Currently, two official plugins are available:
- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Purpose
Testing out publishing with gh pages.  Basic sequence below

~~~
npm install gh-pages --save-dev
~~~
In the vite config file make sure that you have something like this with the name of the repository
~~~
base: "/simple-test",
~~~
then in the package.json file add the follow lines before build:
~~~
"predeploy": "npm run build",
"deploy": "gh-pages -d dist",
~~~

When you want to deploy it to git hub pages:
~~~
npm deploy
~~~

I think I got everything needed in here.  Will have to double check at some point.