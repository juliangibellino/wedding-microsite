# Wedding microsite

## Builds

The build scripts for the project can be located under the `gulp` directory. Each build task has been separated into 
its own file within the `gulp/tasks` directory

For individual tasks, the following can be used:

* Compile View - `gulp compile-view`
* Compile CSS - `gulp compile-sass`
* Compile JS - `gulp compile-js`
* Compile Assets - `gulp compile-assets`
* Dev w/ Live Reload - `gulp dev`
* Build - `gulp build`

### Build Configuration

The configuration of each build task can be found within the individual task files under `gulp/tasks`. To modify 
configuration properties such as source and distribution locations, see `gulp/config.js`. 


### Development build

To build the project locally, follow the following steps

1. `cd` into project directory
2. Run `npm install`
3. Run `gulp build`
4. Once build has successfully ran the project will be distributed to `/dist`

Optionally for production builds the argument `--prod` can be added to minify and uglify output to distribution.

For example when building to production, the following can be used `gulp build --prod`.

### Development build setup with watches and live reload

When working on changes, it is recommended to run `gulp dev` to view up-to-date changes as you work.

To build the application and create local server with changed observed, follow the following steps

1. cd into project directory
2. Run `npm install`
4. Run `gulp dev`
5. Open [http://localhost:3000](http://localhost:3000)


## Source Files

The source files of the project are located under the `src` directory. Each layer of the front-end has has been
separated into the following; however, this structure can be modified for the needs of your project.

* HTML: `src/view`
* JS: `src/js`
* CSS: `src/scss`
* Assets `src/assets` (e.g images, svg, fonts, etc)

Once the project has been built all source files will be compiled to the `dist` directory
