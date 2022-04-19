## For the node.js

### Open the cmd

 ```
 npm install -g heroku
 ```
 ```
 heroku --version
 ```
 ```
 heroku create <app name>
 ```
 
 ```
 git remote -v
 ```
 if it doesn`t have heroku git repository make it.
 ```
 heroku git:remote -a <app name>
 ```
 ```
 git push heroku <branch name>
 ```

※ buildpack 설치가 필요할시
```
heroku plugins:install buildpack-registry
heroku plugins:install buildpacks
```
 
 
 
