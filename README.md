# 📝 Angular-101 📝 
Simple guide to create and publish a Site using Angular

## Step 1: Install Angular!
<code> npm install -g @angular/cli<aio-angular-dist-tag class="pln"></aio-angular-dist-tag> </code>

## Step 2: Starting a new project (in it's own folder)
<code> ng new {name of project} </code>

### You can delete the content of .html and .css inside "app"

## Step 3:
### Development process 1.1
<br> Making sure you are in the folder of the project...
<code> cd {name of project} </code>
<br> Openning a constantly updated version of production
<code> ng serve --open </code>

### Development process 1.2
Use "Nx Console" for Vs Code

## Step 4: Deploying static version in a separated folder
Go to angular.json within the main folder of the project and change the attribute "outputPath" (located in "build") to "docs". This will allow Github down the line to know where to get the Index.html

## Step 5: Keep track of the size
Go to angular.json within the main folder of the project and change the value of "budgets" attributes, specifically
to "maximumError"

# Step 6: Last stage
Run <code>ng build</code> to export a static folder with our App

# Creating a Github repository and updating it
## Step 1: Create a new Repository
## Step 2: Sync our current project
<p>
  <code> git init </code>
  <br><code> git add . </code>
  <br><code> git commit -m 'comment up to you' </code>
  <br><code> git remote add origin {link available at your repo in "Code" button as HTTPS, or initial page of empty Repo} </code>
  <br><code> git branch -M main </code>
  <br><code> git push -u origin main </code>
</p>

## Step 3: Setup Github Pages
Go to "Settings" and click in the "Pages" option, the enable the option and select 'main' as the root to look after and 'docs' for the location of the Index.html


# 🚨 Useful resources 🚨
## In case the app is working fine but leaves a blank page once hosted
https://stackoverflow.com/questions/51718020/when-running-ng-build-the-index-html-does-nothing
Simple trick is just Remove / from the href="/" line from the index.html Change line base href="/" to base href=""
<br>
## In case you want a visual guide
https://www.youtube.com/watch?v=42uxw1Hjo2s&ab_channel=PragmaticReviews 

# 🖥️ Commit future changes 🖥️
<p> 
  <code>git add .</code>
  <br><code>git commit -m "your comment"</code>
  <br><code>git push -u origin main</code>
</p>
