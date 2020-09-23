 1. Plan your gem, imagine your interface
2. Start with project structure
3. Start with the entry point -the file run
4. Force that to build the CLI
5. Stub out the interface
6. Start making thins real
7. Discover objects
8. program

- A command line interface that gives info on the top 50 singers of all time

command line asks  "Would you like to see who the top 50 singers of all time are?"

user types "Yes"

Show a list of artists

Which artist would you like to know more about?
Simply type their name!

Give them info from the site based on the artist..

##negansfavesingers-cli

##-------------------- .bin/console

#!/usr/bin/env ruby

require "bundler/setup"
require "top50singers/cli"

# You can add fixtures and/or initialization code here to make experimenting
# with your gem easier. You can also use a different console, if you like.

# (If you use this, don't forget to add pry to your Gemfile!)
# require "pry"
# Pry.start

require "irb"
IRB.start


##-------------------- .bin/top50singers

#!/usr/bin/env ruby
require './lib/top50singers'

Top50singers::CLI.new.call


##-------------------- ./lib/top50singers


