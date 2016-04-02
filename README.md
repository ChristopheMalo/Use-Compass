# How to use Compass

This project shows different tests with Compass.

I'm working on MAC OS X Lion (10.7).

This project needs to update ruby to 2.0 version or higher.

Due to my old system (MAC OS X 10.7), homebrew can not install Ruby. I use RVM (Ruby Version Manager).

You need homebrew to install gpg2.

You need gpg2 to install RVM.

## Installation
- Upload command line tools from the Apple developer tool (no needs to install x code)
- Install or update hombebrew, [go to official homebrew site](http://brew.sh)
- To update: brew update
- To check the installation: brew doctor
- Follow the recommendation of homebrew before continuing
- Install curl (if it's not on your machine): install brew curl
- Install gpg2: brew install gpg2
- Install key with gpg2: (Follow RVM site)[https://rvm.io/rvm/install]
- Install RVM stable with Ruby (latest version): \curl -sSL https://get.rvm.io | bash -s stable --ruby
- RVM download and build a ruby version
- Restart the console
- Check the ruby version: ruby -v and gem version: gem -v
- Need to reinstall Sass with new ruby (because conflicts between ruby system and ruby RVM): rvm use system - and - gem uninstall sass
- Install fresh Sass: rvm use default (change to new ruby version) - and - gem install sass - and - sass -v (check version - no warning message)
- Install Compass: gem install compass
- Check the version: compass -v

## Memento RVM
- Use the default system ruby: rvm use system
- Display list of local gems: gem list
- Use ruby version installed in machine: rvm use default or [version_number]
- Install specific version: rvm install 2.0.0
- Generate documentation: rvm docs generate-ri

## Memento Compass
- Create the project: compass create [project_name]
