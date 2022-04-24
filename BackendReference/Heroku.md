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

리눅스에서 node.js에서는 사용할 때 uppercase를 적용하면 충돌이 일어날 수 있다는 것을 보고 파일이름을 전부 lowercase로 변경했으나 heroku git remote repository에서는 적용이 안됨 그래서 git mv 와 heroku run bash로 리눅스에 들어가서 mv 명령어를 써도 바뀌지가 않음 그래서 할 수 없이 다시 전부 원래대로 바꿈

Heroku에 .env 파일을 배포하기 위해서는
```
npm i -g heroku-dotenv
```
```
heroku-dotenv push
```
이렇게 하면 heroku-dotenv 가  .env 파일에 저장해 놓은 환경변수들을 연결되어 있는 heroku서버에 전달하고 적용시킴
![jawsdbmaria](https://user-images.githubusercontent.com/73014464/164972954-7c907161-a7d1-4408-9944-2052eb087f9b.png)

 
 
