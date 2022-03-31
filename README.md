# Web app template

This is a web app template with [Parcel.js](https://parceljs.org/) suitable for most of my vanilla JavaScript projects.

## Using this repository to start a new project

1. In GitHub, click the `Use this template` button.
1. Follow the instructions to create a new repository from `web-app-template-parceljs`.
1. Clone the newly created repository.
1. Update the following values in the `package.json` file:
   - `name`
   - `description`
   - `public-url` parameter used in the `build` script. It should match your newly created repository name.
1. Run `npm install` to download the dependencies. It should create the `node_modules` folder and update the `package-lock.json` file.
1. Update the contents of the `README.md` file:
   - Update the title.
   - Add a brief description of the project.
   - You can probably remove the section `Using this repository to start a new project`, as it's only meaningful for this template.
1. Commit and push these changes.
1. You are ready to start the development!

## Running the app for development

1. Run `npm install` to download the dependencies. The `node_modules` folder will be created.
1. Run `npm run start` to start a server at `http://localhost:1234`.
   - Parcel.js will build the application and make the artifacts available in the `dist` folder.
   - The SCSS files will be converted to CSS files.
   - Chrome will open a new tab, displaying the application.
   - As the application is developed, Parcel.js will watch for code changes, and will instruct the browser to reload the page. Like magic!
   - The contents of the `dist` folder are deleted by Parcel.js. So the contents of the `dist` folder must not be touched!

## Building the app

Run `npm run build` to build the application. The application artifacts will be available in the `dist` folder.

## Deploying the app in Netlify

1. Open Netlify: [`https://app.netlify.com`](https://app.netlify.com).
1. Under the _Sites_ section, click the _Add new site_ button, and select _Import an existing project_.
1. Select _GitHub_. Grant access to Netlify if necessary.
1. Pick this repository from the list.
1. Review the site settings. You'll most likely want to deploy from the `main` branch.
1. Click the _Deploy site_ button.
1. Wait until the deploy completes (refresh the page if necessary).
1. Netlify will create a site name such as `clever-dasik-b326ad`. It will also create a URL like `https://clever-dasik-b326ad.netlify.app`. To modify it, click the _Site settings_ button, and then click the _Change site name_ button.
1. To make this content available under `https://portfolio.claucia.com` or `https://claucia.netflify.app`, update the [`_redirects`](https://github.com/claucia/portfolio-netlify/blob/main/_redirects) file in the [`portfolio-netlify`](https://github.com/claucia/portfolio-netlify) repository.
1. When changes are pushed to GitHub, Netlify will automatically build and deploy them.
