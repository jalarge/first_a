
## Ruby on Rails: first_a ... playing around with github and heroku. Thanks Hartl

A mashery [markdown cheat sheet](http://support.mashery.com/docs/customizing_your_portal/Markdown_Cheat_Sheet).

## Create this project.

From a project directory containing a project Gemfile and project .gitignore file.
				$ rails new first_a
				$ cd first_a
				
				$ git init
				-> $ mate .gitignore or $ cp ../.gitignore .
					$ git status
				$ git add .
				$ git commit -m "rails new first_a"
					$ git log

				-> $ mate Gemfile or $ cp ../Gemfile .
				$ bundle install
				$ rails s
				-> localhost:3000

					$ git status
				$ git add .
				$ git commit -m "Update of Gemfile for env : os x, textmate, iTerm2, rails 3.2.2"
					$ git log

				-> login to GitHub & create new repository first_a
				$ git remote add origin git@github.com:jalarge/first_a.git
				$ git push origin master

					$ git branch
				$ git checkout -b modify-README

				$ git mv README.rdoc README.md
				$ mate README.md

				$ git status
				$ git commit -a -m "Updated the README to a markdown file."
				$ git checkout master
					$ git branch -D topic-branch (if major branch screwup.)
				$ git merge modify-README
				$ git branch -d modify-README

				$ git push

				$ gem install heroku
				$ heroku keys:add
				$ heroku create --stack cedar
				$ heroku open
				
				