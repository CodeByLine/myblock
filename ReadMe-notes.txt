About the folder "node-modules" (advice fr Reddit):

The node_modules shouldn’t be in your repository if you are using git. It should be added to the .gitignore;

if the package.json is saved to github yes. you can always npm install from it in the future;

Make sure to commit package-lock.json as well, since otherwise you could get conflicts or things breaking if you try to install in the future

while most of the size will come from modules you use for development only, some might be necessary to run it. You should look up npms dependencies VS devDependencies.