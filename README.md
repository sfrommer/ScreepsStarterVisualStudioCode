## Starting template for Screeps Workspace in Visual Studio Code

This repo is intended to create a Workspace in VS Code. It features autocompletion and you can copy your scripts to your local Screeps Folder(s) with Gulp. 
Because local folders are used, this Workspace is only suitable if you play using the Steam Client. It is possible to use without it, though. Check the bottom of this page if you're interested in that.

---
### Setup Instructions

1. **Install Nodejs** (https://nodejs.org/en/download/)

2. **Install typings** (https://www.npmjs.com/package/typings):
 ```
 npm install typings --global
 ```
3. **Install gulp** (https://gulpjs.com/):
 ```
 npm install gulp-cli -g
 ```
4. Do the following commands **inside your project folder** (the integrated terminal in VS Code is nice for that)
 **Initialize your project** (Give your project a name, for example "screeps". Press enter until you reach the last question, then type "yes"...):
 ```
 npm init
 ```
 **Add Gulp to your Project:**
 ```
 npm install gulp -D
 ```
5. **Set the path constants** to your local screeps folder(s) **in "gulpfile.js"** (You can find your local path by clicking the "Open local folder" button in the Screeps Console of the Steam Client)

---

### How to write Scripts and deploy with Gulp
Place all your game scripts in the "scripts" folder (Already existing Scripts are from the Tutorial).
All .js files are copied to your Screeps Folders (PATH you had set up in gulpfile.js) each time you use the following commands:

 ```
 gulp deploy_1
 ```
 or
 ```
 gulp deploy_2
 ```
---

### Possible improvements of this Workspace

 Recommended VS Code Extensions:

+ Gulp Tasks -> if you prefer to deploy over a GUI Button instead of a Console Command

---
**Push to the official Server with Gulp**

If you want to use Gulp to push to the official Server consider implementing this: https://www.npmjs.com/package/gulp-screeps.
It allows you to deploy your scripts to the official Server without the Steam Client and its local files.
