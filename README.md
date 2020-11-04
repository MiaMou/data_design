# README for the DataDesign > #
Ruby 2.6.3  Rails  6.0.3.4
A live version is deployed on Heroku, and can be accessed using the following link:
https://nameless-journey-04654.herokuapp.com/

# The bugets and funds of world bank（2015-2021）
This is a Ruby on Rails app based on the World Bank Program Budget And All Funds FY15-FY21 found at https://finances.worldbank.org/Budget/World-Bank-Program-Budget-and-All-Funds-FY15-FY21/9g9y-b7rs 

## Charts
Echarts are used for generating charts

### Move to Postgresql Locally
While generating JSON the SQL language differences between SQLite3 and Postgresql made it necessary to shift local development to Postgresql. Making changes, and then pushing them to Heroku takes too long (4-5 minutes each cycle due to recompiling of assets), so running Postgresql locally is important.
In order to do this with Postgresql, you need to (a) set up a database to use, (b) assign an 'owner' and password for the database, whose details you put into the config/database.yml file, then you can (c) run your migrations and any rake tasks to seed the database, (d) change the gemfile to use 'pg' gem for development, test, and production and then run 'bundle install'. Now you can start to work with Postgresql locally and remotely. 

### Build JSON with Jbuilder

## Bootstrap
We use Bootstrap to clean up the look and feel of the application. 

## running the application locally ##
1. bundle install
2. rails db:create
3. rails db:migrate
4. rails import:data
5. rails server

Access the application using:http://localhost:3000
Group Members
Zhewei Huang (51989960)
Danping Mou (51989963)
Yu Xing（51990018）

## These are the parts that are not working correctly ##
We tried to link map in out application but failed.

