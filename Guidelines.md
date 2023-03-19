The procedure to create a React app, connect to GitHub and then deploy on Firebase

The references used:

https://blog.logrocket.com/deploying-react-apps-github-pages/#pushing-the-react-app-to-the-github-repository

Above reference is used to create the app, create github repo, and then connect to GitHub repository


https://medium.com/swlh/how-to-deploy-a-react-app-with-firebase-hosting-98063c5bf425

Above ref to connect React project to Firebase. This reference does not cover the details of connecting GitHub to firebase to automate the continuous deployment


Steps:

1. Create a repository in GitHub

Go to your profile and create a repository +

2. Create a react project

npx create-react-app "your-project-name"

3. Test the react app

Cd XXX
Npm start

4. If not done yet, generate RSA key on your computer and copy the public key on GitHub

5. Initiate your git in the local project and make the the first push

git init

git commit -m “some message”
git branch -M main
git remote add origin https://github.com/nelsonmic/testxx.git (copy from Github repository)
git push -u origin main

Firebase 

6. Install Firebase package locally

npm install firebase-tools -g

7. You will need a firebase account, and create a project on the firebase website

firebase login

firebase init
firebase deploy


