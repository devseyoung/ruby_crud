# How to build

rails new PROJECT_NAME
rails new homework

cd homework

git init => to initial commit
rails s => run server , check if it is working

### install gem

[rubygems](https://rubygems.org/)
=> to check current version of gems

Make errors better looking

gem 'better_errors', '~> 2.5', '>= 2.5.1'

Bulma CSS

gem 'bulma-rails', '~> 0.8.0'

Simple Form

gem 'simple_form', '~> 5.0', '>= 5.0.1'

group :development do

Guard is a command line tool to easily handle events on file system modifications.

gem 'guard', '~> 2.16', '>= 2.16.1'

Guard::LiveReload automatically reloads your browser when 'view' files are modified.

gem 'guard-livereload', '~> 2.5', '>= 2.5.2'
end

bundle (terminal) => to run added gems

how to use gems that I add => search documents for them

[document for simple_form gem](https://github.com/plataformatec/simple_form)

### rails g controller posts => it should be plural for the controller, but for the model it should be singular

=> set up after generating controller

1. controller
2. route
3. show, create, edit, update, destroy

### generate Data model (database)

1. rails g model Post title:string content:text
2. rails db:migrate
   To see all crud action
3. rake routes
