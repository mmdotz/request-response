#Request-Response


##Description
Access a users table in the database. Users have first_name, last_name, and age attributes.

##Features
Show the users with certain parameters, via a `GET` request.

##Instructions
To see ALL the users from the database printed out with an appropriate response codes:
`GET` : at http://localhost:3000/users HTTP/1.1

To see ONLY the user from the database with a certain id:
`GET` : at http://localhost:3000/users/1 HTTP/1.1

To see a message saying the user was not found along with the appropriate response code.
`GET` : at http://localhost:3000/users/9999999 HTTP/1.1


## Rundown

```
.
├── Gemfile             # Details which gems are required by the project
├── README.md           # This file
├── Rakefile            # Defines `rake generate:migration` and `db:migrate`
├── config
│   └── database.yml    # Defines the database config (e.g. name of file)
├── console.rb          # `ruby console.rb` starts `pry` with models loaded
|__ bin
    |__ run.rb          # Run this file using Ruby version 2.2.3
├── db
│   ├── dev.sqlite3     # Default location of the database file
│   ├── migrate         # Folder containing generated migrations
│   └── setup.rb        # `require`ing this file sets up the db connection
└── lib                 # Your ruby code (models, etc.) should go here
    └── all.rb          # Require this file to auto-require _all_ `.rb` files in `lib`

```
