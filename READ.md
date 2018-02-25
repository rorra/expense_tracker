# How to change the environment

Just use the Environment Variable RACK_ENV, with either development, test or
production, like

    RACK_ENV=test bundle exec ...

# Creating the DB

Run

    bundle exec sequel -m ./db/migrations sqlite://db/development.db --echo
