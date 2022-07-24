## Portfolio Website V2-Overview

### Process
- The first version of my portfolio website was built in 2019 
- To use this website as a tempalte for your portfolio, follow the instructions below 
- Begin by choosing a color theme and collecting all of the relevant assets needed including images 
- The current version is using a web3 inspired design language using colors from Material Design's dark theme guide
-The original website was a clone of public ror site, the current website has changed substantially since V1

### Portfolio Contents
-	Bio
-	Education
-	Work History (some of, the most recent)
-	Key attributes
-	Portfolio content
-	Contact form (inactive, available schema/logic)

#### Tech used and integrations
- Ruby On Rails
- JQuery
- Javascript
- Google analytics & Tag Manager
- HTML 
- SASS 
- Bootstrap 
- Google font API 
- Font Awesome 
- Mailer - Contact Mailer 
- Hosting: Heroku


___________
## Installation 

### Clone the repository

```shell
git clone git@github.com:TaylorJalpha/portfolio_master
cd project
```
___________
### Verify your Ruby version

```shell
ruby -v
```
The ouput should start with something like `ruby 2.6.3`

If not, install the correct ruby version using [rbenv](https://github.com/rbenv/rbenv) (remain calm, it may take a while):

```shell
rbenv install 2.6.3
```
___________
### Install dependencies

Using [Bundler](https://github.com/bundler/bundler) and [Yarn](https://github.com/yarnpkg/yarn):

```shell
bundle && yarn
```
___________
### Initialize the database
```shell
rails db:create db:migrate db:seed
```
___________
### Set environment variables
#### Puma ENV Variable (current config- Puma.rb)
```port        
ENV.fetch("PORT") { 9292} 
```
Change to default if prefered
```port        
ENV.fetch("PORT") { 3000} 
```
___________
### Add heroku remotes

Using [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli):

```shell
heroku git:remote -a project
heroku git:remote --remote heroku-staging -a project-staging
```
___________
### Serve-Start Puma Web Server

```shell
rails s
```

### localhost 

```shell
https://localhost:3000 
```
Confirm ```ENV.fetch("PORT") { 3000}``` source ```puma.rb```
___________
### Deploy

#### With Heroku pipeline (Optimal)

Push to Heroku staging remote:

```shell
git push heroku-staging
```

Go to the Heroku Dashboard and [promote the app to production](https://devcenter.heroku.com/articles/pipelines) or use Heroku CLI:

```shell
heroku pipelines:promote -a project-staging
```
___________
### Heroku production (Ship it! when ready)

Push to Heroku production remote:

```shell
git push heroku 
```
Branch-specific push to Heroku:

```shell
git push heroku {branch-name} 
```
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]
(https://opensource.org/licenses/MIT)
