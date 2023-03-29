** If u have any problems with file pathes, here is the link to w3schools with explanation:
https://www.w3schools.com/html/html_filepaths.asp

1. "npm init -y" - to init a package.json
2. "npm i --save-dev typescript" - to install ts
3. "npm tsc --init" - to create a config file
4. now u can change the settings as in Mosh-Tutorial if u need.
5. create a src folder for index.ts
6. change in tsconfig.json setting for compiled js file: "outDir": "./dist",
7. activate sourcemap for js file: "sourceMap": true,
8. u can create a command in package.json to automaticlly compile a ts file: "scripts": {
    "start": "tsc --watch"
  }, and then: "npm start" to start a package.json with new settings
9. U can run a code of js file in terminal with node dist/index.js or where the file is... So u don't need to go live or do it in console.
10. enable noUnusedLocals, noUnusedParameters, noImplicitReturns = true in tsconfig
11. when u run and debug u need to create launch.json and there u put and extra setting after a program setting: "preLaunchTask". And then the followed string with the value: "tsc: build - tsconfig.json"
12. "sourcemap" - must be on in tsconfig.json for debbuger