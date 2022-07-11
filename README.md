# https://portfolio.TaylorFerguson.xyz
<div id="header" align="center">
  <img src="https://media.giphy.com/media/5P5b96VnFaNiQ7ABOT/giphy.gif" width="100"/>
</div>

<h1 align="center">
  Hello, I'm Taylor 
</h1>

### About Me :

I'm a Web Developer, Product Manager, and Technical Writer based in Los Angeles, CA

- :microscope: I work as a Web Developer(web2) & Product Manager for a multiple projects(web3), and formerly a PM for web2 saas companies (b2b + b2c), primarily - My goal is to pivot away from product to focus on dev, indeally within a high-growth startup while continuing to refine my product and management skills 

- :memo: During my freetime I freelance as a Technical Writer - :rocket: <b>Goal:</b> refine writing skills to support content-strategies and content creation

- :sunrise_over_mountains: When I'm not working, I explore the mtns, ride bikes and run/hike trails

- :pager: Let's connect!: [![Linkedin](https://i.stack.imgur.com/gVE0j.png) LinkedIn](https://www.linkedin.com/in/taylor-ferguson-57826660/)
&nbsp; [![GitHub](https://i.stack.imgur.com/tskMh.png) GitHub](https://github.com/taylorJalpha)

---

### :musical_score: Tech Used :

<div>
  
   <img src="https://github.com/devicons/devicon/blob/master/icons/ruby/ruby-original-wordmark.svg" title="Ruby" alt="Ruby" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/rails/rails-original-wordmark.svg" title="Rails" alt="Rails" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/javascript/javascript-original.svg" title="JavaScript" alt="JavaScript" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/graphql/graphql-plain-wordmark.svg" title="GraphQL" alt="GraphQL" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/nodejs/nodejs-original-wordmark.svg" title="NodeJS" alt="NodeJS" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/heroku/heroku-original-wordmark.svg" title="Heroku" alt="Heroku" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original-wordmark.svg" title="docker" alt="docker" width="40" height="40"/>&nbsp;
</div>

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=taylorjalpha&theme=radical)](https://github.com/anuraghazra/github-readme-stats)

--- 

## Portfolio Website V2-Overview

### Process
- The first version of my portfolio website was built in 2019 
- To use this website as a tempalte for your portfolio, follow the instructions below 
- Begin by choosing a color theme and collecting all of the relevant assets needed including images 
- The current version is using a web3 inspired design language using colors from Material Design's dark theme guide

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
- SCSS 
- Bootstrap 
- Google font API 
- Font Awesome 
- Mailer - Contact Mailer 
- Hosting: Heroku
- CDN: UNPKG


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
