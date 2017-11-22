
I created some updates to the course to help smooth along the examples. 

Since I created this course, a few libraries have changed where they did not follow semver (semantic versioning). We cannot control that, but we can make fixes :)

Option 1: Manual Changes

1. Change all ^ to ~ in the package.json file (this tells npm to get only patch updates, not minor updates)
2. Change karma-phantomjs-launcher in package.json to ~1.0.4
3. Change phantomjs in package.json to ~2.1.7
4. Change bootstrap in the bower.json file to the exact version 3.3.1 (no tilde, no caret) (bootstrap changed their main file, which the gulpfile relies on)
5. delete your node_modules and bower_components folders, and re-run npm install and bower install

Option 2: Refer to the final JSON files

The updated package.json and bower.json files in this folder use the versions that will work with the course. 



Thanks for watching, and enjoy gulp!

John Papa