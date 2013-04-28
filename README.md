# Rails Starter App

A starter application, taken from the Rails 4.0 Tutorial up through Chapter 9. 

Includes user resource, authentication/authorization and plenty of rspec tests.

This code is from the sample application for
the [*Ruby on Rails Tutorial*](http://railstutorial.org/)
by [Michael Hartl](http://michaelhartl.com/).

To set up:
<pre>
git clone https://github.com/sloanahrens/starter_app.git [newappname]
cd [newappname]
git remote rm origin
git remote add origin https://github.com/[username]/[newappname].git
git config master.remote origin
git config master.merge refs/heads/master
[create repo]
git push -u origin master
bundle install
bundle exec rake db:migrate
bundle exec rake db:populate  # if you want some dummy users
bundle exec rake db:test:prepare
bundle exec rspec spec
unicorn_rails -p 3000
</pre>