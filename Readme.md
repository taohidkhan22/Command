## Command


### Git repository creation on local computer 
1. mkdir "folder name" <br>
2. git init <br>
3. add, commit<br>
4. git remote add origin "remote repo link"<br>
5. git remote -v(for checking the repo)<br>
6. git branch<br>
7. git push origin main or git push -u origin main
   
### React App creation using vite
1. npm create  vite@latest
2. Select: React-> Javasript
3. Command line:<br>-cd Redux
  <br>-npm install
  <br>-npm run dev <br>
4.  Creating style using style.scss file -> npm install -D sass
### Github blank page issue
1.  'vite.config.js' "base": "/Your RepoName/"
2.  'package.json' "homepage": "https://YourAccountName.github.io/YourRepoName"
3.  git add .
4.  git commit -m"your meesasage"
5.  git push
6.  npm run build
7.  npm run dev
8.  npm run preview(Before deploying into GitHub you can actually see in your local browser how your page will work on GitHub)
9.  npm run deploy (Deploying Github)<be> 

Note: _if you have picture issues like (Everything working fine on your website. In your GitHub page picture is not loading, then you have to import the picture in your specific component)_
- Example:
```
       <import image_name from '../assets/images/image.png'; [into your .jsx file]
         <img
                  src={image_name}
                  width="__"
                  height="__"
                  style={{ marginLeft: "0px" }}
                  alt=""
         />
```
### 'Script' for package.json

```
"predeploy": "npm run build",
    "deploy": "gh-pages -d dist",
    "dev": "vite",
    "build": "vite build",
    "lint": "eslint . --ext js,jsx --report-unused-disable-directives --max-warnings 0",
    "preview": "vite preview"
```
### Fork a GiTHuB Repo:
1. git clone https://github.com/your-username/forked-repo.git
2. git remote add upstream https://github.com/original-owner/original-repo.git
3. git fetch upstream
4. git merge upstream/main
5. git push origin main
