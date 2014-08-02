Ruby on Rails project running on linux and deployed to heroku.

1. Set up development's Ruby on Rails environment

- Get an update for the latests available packages 
sudo apt-get update         

- Download the curl package to make web requests through the terminal
sudo apt-get install curl   

- Get RVM on its website and execute it
\curl -L https://get.rvm.io | bash -s stable   

- Exit the terminal, open a new one again and load RVM 
source ~/.rvm/scripts/rvm

- Install RVM dependencies 
rvm requirements

- Install ruby through rvm
rvm install ruby

- Install rubygems (packages and libraries)
rvm rubygems current

- Install Rails
gem install rails


2. Set up heroku command line and tools 
wget -qO- https://toolbelt.heroku.com/install-ubuntu.sh | sh

3. Create a heroku project (You have to create a heroku account first)

- Login to your account through the terminal:
heroku login

- Create a new project environment
heroku create [project-name]

- Create a repository with github
git init
git add .
git commit -m "Your message"

- Push the repository to heroku
git push heroku master


EXTRAS:
To run this repository:
git clone https://github.com/AAlvAAro/phonebook
cd phonebook
bundle exec rails server


