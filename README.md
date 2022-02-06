# Web app template

This is a web app template with [Parcel.js](https://parceljs.org/) suitable for most of my vanilla JavaScript projects.

## Cloning the repository for starting a new project

The steps below describe how to clone this repository for starting a new project, keeping the history.

1. On GitHub, create a repository. To illustrate, let's call it `my-new-web-app` 
1. Open Terminal.
1. Create a folder for the project, matching the repository name: `md my-new-web-app`.
1. Enter the newly created folder: `cd my-new-web-app`.
1. Clone the template repository into the newly created folder: `git clone https://github.com/claucia/web-app-template-parceljs.git .` (don't forget the `.` at the end, as it indicates the current folder).
1. Change the remote URL in the local repository: `git remote set-url origin https://github.com/claucia/my-new-web-app.git`.
1. Push the files to the remote repository: `git push`.
1. In GitHub, check if the files have been corretly pushed to the repository.
1. Still in Terminal, open the folder in Visual Studion Code: `code .`.
1. Update the follow values in the `package.json` file:
   - `name`
   - `description`
   - `public-url` parameter used int the `deploy` script (it should match your new repository name: `/my-new-web-app`).
1. Update the contents of the `README.md` file:
   - Update the title.
   - Add a brief description of project
   - You can probably remove the section `Cloning the repository for starting a new project`, as it's only meaningful for this template.
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

## Deploying the app in GitHub Pages

1. Run `npm run deploy` to build and deploy the application in GitHub Pages. The application artifacts will be available in the `dist` folder, and then copied to the `gh-pages` branch. 
1. Push the changes to GitHub. The `gh-pages` branch will be used by GitHub Pages to make the static content available in the web.
