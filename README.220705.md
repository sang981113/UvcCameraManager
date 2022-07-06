1. ndk set to android-ndk-r16b-windows-x86_64
URL: https://github.com/android/ndk/wiki/Unsupported-Downloads

2. npm install metro-config
for make bundle in ./android/app/src/main/assets

3. encountered error
Unable to load script from assets 'index.android.bundle'. Make sure your bundle is packaged correctly or you're running a packager server

URL: https://stackoverflow.com/questions/44795384/unable-to-load-script-from-assets-index-android-bundle-make-sure-your-bundle

If it shows [React-Native] SyntaxError: Invalid regular expression,
you should downgrade your nodejs version to 12.10.0 using nvm.

4. If it shows code ENOLOCAL, when you did npm install.
DELETE YOUR package-lock.json FILE IN YOUR PROJECT.

    npm install  

npm ERR! code ENOLOCAL
npm ERR! Could not install from "node_modules\react-native-scrollable-tab-view\react-native-viewpager@git+https:\github.com\ge6285790\react-native-viewpager.git#3b04539" as it does not contain a package.json file.

5. react-native run-android occurs error THIS
error: bundling failed: ambiguous resolution: module `C:\Users\sang9\AndroidStudioProjects\UvcCameraManager\index.android.js` tries to require `react-native`, but there are several files providing this module. You can delete or fix them:

    react-native start --reset-cache

