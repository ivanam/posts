# RailsMySQL
Sample Application on Ruby on Rails 5 using MySQL


* Ruby version 2.6.0


* Configuration

To config this app you need run:

 
# Adding Node.js 10 repository


curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -


# Adding Yarn repository

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -

echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

sudo add-apt-repository ppa:chris-lea/redis-server


# Refresh our packages list with the new repositories

sudo apt-get update


# Install our dependencies for compiiling Ruby along with Node.js and Yarn

sudo apt-get install git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev software-properties-common libffi-dev dirmngr gnupg apt-transport-https ca-certificates redis-server redis-tools nodejs yarn


#Installing ruby 2.6.0 with rbenv...

git clone https://github.com/rbenv/rbenv.git ~/.rbenv
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
echo 'eval "$(rbenv init -)"' >> ~/.bashrc
git clone https://github.com/rbenv/ruby-build.git ~/.rbenv/plugins/ruby-build
echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
git clone https://github.com/rbenv/rbenv-vars.git ~/.rbenv/plugins/rbenv-vars

exec $SHELL
rbenv install 2.6.0
rbenv global 2.6.0
ruby -v



#install bundler 

gem install bundler



# For older apps that require Bundler 1.x, you can install it as well.

gem install bundler -v 1.17.3



# Test and make sure bundler is installed correctly, you should see a version number.

bundle -v



#Repo

clone the repo https://github.com/ivanam/posts.git



#Database creation

rake db:create

rake db:seed

rake db:seed


#run the app

rails s

