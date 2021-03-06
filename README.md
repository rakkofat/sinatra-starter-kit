# Sinatra Active Record Starter Kit

This template provides a basic [Sinatra](http://www.sinatrarb.com/) application
that includes:

- [Active Record](http://guides.rubyonrails.org/active_record_querying.html)
using [sinatra-activerecord](https://github.com/janko-m/sinatra-activerecord)
- [PostgreSQL](http://www.postgresql.org/) for a database
- [Sinatra::Reloader](http://www.sinatrarb.com/contrib/reloader.html) to
  automatically reload modified files during development
- [RSpec](https://github.com/rspec/rspec) for unit testing
- [Capybara](https://github.com/jnicklas/capybara) for acceptance testing
- [Pry](https://github.com/pry/pry) for debugging
- [Foundation 6](http://foundation.zurb.com/sites.html) with flex grid for styling
- [lodash v3.10.1](https://lodash.com/) for easier javascripting.

## Configuring Your Database

This template is set up for using a PostgreSQL database. You will need to edit the
`config/database.yml`.

You can create your database with
`rake db:create`.

## Rake Tasks

This template uses the [sinatra-activerecord](https://github.com/janko-m/sinatra-activerecord)
gem, which provides the following rails-like rake tasks:

```no-highlight
rake db:create            # create the database from config/database.yml from the current Sinatra env
rake db:create_migration  # create an ActiveRecord migration
rake db:drop              # drops the data from config/database.yml from the current Sinatra env
rake db:migrate           # migrate the database (use version with VERSION=n)
rake db:rollback          # roll back the migration (use steps with STEP=n)
rake db:schema:dump       # dump schema into file
rake db:schema:load       # load schema into database
rake db:seed              # load the seed data from db/seeds.rb
rake db:setup             # create the database and load the schema
rake db:test:prepare      # Prepare test database from development schema
```
