== README

This README would normally document whatever steps are necessary to get the
application up and running.

Topics of interest:

## To kill threads that take up memory...the spring server and app
* ps aux
* kill -9 PID

## Environments:
* Ruby version: 2.2.1-p85 (x86_64-linux)
* Rails version: 4.2.4
* RubyGems version 2.4.6
* Rack version 1.6.4

#Note: to see the site live on the internet type in terminal: #
`rails s -b $IP -p $PORT`
    
## For Github to push:
* git push origin master --force <- should only be needed once
* git push -u origin --all

## Dual push
To Push to both github and bitbucket :) Yay...this is awesome
* http://blog.lckymn.com/2013/03/11/git-push-to-pull-from-both-github-and-bitbucket/

## Prep github
`git checkout static-pages`
`git checkout -b static-pages-exercises`

## Solving Exercises

* see branch for static-pages-exercises
`git commit -am "Eliminate repetition (solved)`
`git add -A`
`git commit -m "add page"`
`git push -u origin static-pages-exercises`
`git checkout master`


To deploy to heroku
* `heroku create` <- at the terminal ***ONLY ONCE***
* `git push heroku master`

To create a branch: 
* `git checkout -b nameof-pages`
* `git git checkout -b nameof-pages`

To add to a repo:
* `git status`
* `git add -A`
* `git commit -m "add a static page folder"`
* `git push -u origin static-pages`



System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...


Please feel free to use a different markup language if you do not plan to run
<tt>rake doc:app</tt>.
