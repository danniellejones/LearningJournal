# Learning Journal Week 09

## CSS Pre-processing with Sass

**Weekly Objectives:**

- [ ] Create small website using Sass
- [ ] Group project: finalise decisions regarding layout, css/sass, content, planning, workflow (if able)

**Stand-Up Meeting:** <br>
[25/04/2023 - Meeting 05]()

**Team Project:** <br>
[GitHub - Team04](https://github.com/cp3402-students/cp3402-2023-a2-team04)

### Learning Activity

Sass <br>
[Sass Essential Training 2015](https://www.linkedin.com/learning/sass-essential-training/welcome?u=2223545) <br>
[Sass In 100 seconds](https://www.youtube.com/watch?v=akDIJa0AP5c)<br>
[Sass Tutorial for Beginners - CSS With Superpowers](https://www.youtube.com/watch?v=_a5j7KoflTs)<br>
[Stop using an extension to compile Sass](https://www.youtube.com/watch?v=o4cECvhrBo8) <br>
[Sass / SCSS COMPLETE Tutorial (+ Node.js & NPM) with Real-World Example](https://www.youtube.com/watch?v=ztEY-uber4U) <br>
[What is NPM, and why do we need it? | Tutorial for beginners](https://www.youtube.com/watch?v=P3aKRdUyr0s) <br>
[Browsersync + Sass + Gulp in 15 minutes](https://www.youtube.com/watch?v=q0E1hbcj-NI) <br>
[Sass @import is being replaced with @use and @forward](https://www.youtube.com/watch?v=dOnYNEXv9BM) <br>
Estimated Time: 6h 30m

#### Content Insights:

On watching the LinkedIn video on Sass training, as a beginner course I felt it started out beyond my level of
understanding for just the setup. I instead referred to other tutorial videos to see if I could piece together an
understanding of how the setup for Sass worked. Each video I looked at used a sass compiler extension, which was not
what I was trying to understand. The video 'stop using an extension to compile Sass' gave a clear explanation of why not
to use extensions (robustness and updates), but the alternative option offered did not involve gulp like the other
LinkedIn courses had presented. The last video I watched on NPM made everything so much clearer. It suggested commands
like node -v and npm -v to check the version setup. This was important for me to understand as I had other programs that
had node.js that my PHPStorm was using and had trouble working out why they were different from my global cmd versions.

**Important Takeaways:**

Install node.js

* Node.js contains npm package manager and is used to compress sass to css for website use

Installation of packages from npm: locally (project) or globally (all) <br>

* Go to terminal in IDE (PHPStorm), it will be cd to the project folder:
    * Local installation, go to terminal in project folder in IDE
      `npm install sass` <br>
    * Global installation `npm install -g gulp-cli` <br>

The package.json File

* Tracks multiple packages installed, and stores information about your project: name, version, repository and author
  information

* A project with a package.json and run `npm install` will read the package.json file and install all the required
  packages, this is useful for deployment
* Create package.json file `npm init`, answer the questions or fill in after
* Dependencies are listed in the package.json files and are found in node_modules folder
    * Some packages are dependent on other packages, so if there are more packages than expected it is likely because of
      a dependency within their package.json file
    * Package version updates can cause issues, be wary `npm view sass versions`. They follow semantic versioning
      _major:minor:patch_, where major version changes can potentially break code. The symbol ^ limits auto-updating
      to a major version that will break. Update all: `npm update` Update to latest/version: `npm install sass@latest`.
* A package-lock.json exists because of capability issues.

Gulp <br>

* Install gulp globally and locally: `npm install -g gulp-cli`
* Npm to create package.json file, -y indicates to use defaults`npm init -y`
* Install packages locally (project): `npm install gulp gulp-sass gulp-postcss cssnano gulp-terser browser-sync` _note:
  not all are required it is just a suggestion of packages to use_
    * gulp
    * gulp-sass - compile sass files to css
    * gulp-postcss - uses cssnano (post css plugin)
    * gulp-terser - minimises javascript file
    * browser-sync - auto-syncs browser throughout development
* Create `gulpfile.js`, example below:

```
const { src, dest, watch, series} = require('gulp');
const sass = require('gulp-sass');
const postcss = require('gulp-potcss');
const cssnano = require('cssnano');
const terser = required('gulp-terser');
const browsersync = require('browser-sync').create();

//Sass task
function scssTask() {
    return src('app/scss/style.scss', {sourcemaps: true})
        .pipe(sass())
        .pipe(postcss([cssnano()]))
        .pipe(dest('dist', {sourcemaps: '.'}));
}
        
// JavaScript Task
function jsTask() {
    return src('app/js/script.js', {sourcemaps: true})
        .pip(terser())
        .pipe(dest('dist', {sourcemaps: '.'}));
}

// Browsersync Tasks
function browsersyncServe(cb) {
    browsersync.init({
        server: {
            baseDir: '.'
        }
    });
    cb();
}

function browsersyncReload(cb){
    browsersync.reload();
    cb();
}

// Watch task
function watchTask() {
    watch('*.html', browsersyncReload);  // Reload if changes in html files
    watch(['app/scss/**/*.scss', 'app/js/**/*.js'], series(scssTask, jsTask, browsersyncReload));
}


// Default gulp task
exports.default = series(
    scssTask,
    jsTask,
    broswersyncServer,
    watchTask
);
* ```

* Once gulp file is set up, run command: `gulp`

**Returning to the LinkedIn Video and comparing to Sass Information/Website:**

* Information provided in the video about which Sass to use is out-dated - we should be using Dart Sass for new projects
* [Dart Sass](https://sass-lang.com/dart-sass) does not require a wrapper
* Dart has a stand-alone command-line executable which is faster, but to fit into workflows it has a Javascript sass
  package on npm `npm install --save-dev sass and require()`
* There are multiple ways to set up the gulp file, this will need to be compared based on using WordPress or what
  packages are used
* Use of @import is out-dated, @use @forward should be used instead - for learning purposes this may be difficult to
  start with

**LinkedIn Video Key takeaways:**

The objective watching the rest of the video was to be aware of what is possible. Further practice is required to make
use of these elements.

* (Partials) Append files with _ underscore at the start for those that will be imported
* (mixins) Functions, add into file mixin @mixin name(parameter) { function body}, call using @include name(parameter)
* (@extend) inheritance
* (&) Reference parent selectors
* (Comments) /*! */ to show up in compressed version, generally comments //
* Complement, lighten and darken help with colour modifications
* (List) Separated by commas or spaces - list of elements - starts at 1 as first element
* (@content) Combine in a mixin to create break points
* (args...) mixins can handle any number of parameters
* (@for), (@each) and (@while) loops
* Map - dictionary
* Refer to Sass documentation for further information

<br>

#### Career/Employability/Learning Insights:

The new content we are being introduced to in this subject is becoming quite heavy. Every step in information technology
appears connected to something else, which means it is never a simple process. Also, there is a lot of assumed prior
knowledge and I feel like that is where I am struggling to understand many of these courses that expand on this prior
knowledge. Even though it takes longer, I need to approach each of these topics at the level that I understand and build
upon this knowledge. I found [this](https://www.youtube.com/watch?v=s6dMWzZKjTs) video enlightening on this subject. It
discussed not learning things randomly, but with a roadmap focusing on one topic at a time.

As front-end development was one of the fields I was interested in as a career option, it was important to me that I
understood each of the steps in the Sass LinkedIn tutorial. Furthermore, I thought it was important that I had a better
understanding so that I could re-iterate this new understanding to my group if they needed further clarification, as
this was my assigned group role (front-end).