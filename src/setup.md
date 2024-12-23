# Alternate setup instructions

## Create user with password
`CREATE USER '<DB_USER_NAME>'@'localhost' IDENTIFIED BY '<PASSWORD>';`

## Grant all privileges on WelcomeHomeDB to the user
`GRANT ALL PRIVILEGES ON WelcomeHomeDB.* TO 'DB_NAME'@'localhost';`

## Grant FILE privilege for handling images
`GRANT FILE ON *.* TO 'DB_NAME'@'localhost';`

## Apply the privileges
`FLUSH PRIVILEGES;`

## Image upload instructions
- You need to have an `images` directory outside i.e. parallel to your git repo. And that should have all the images.

## DB config instructions
- You need to have `config.py` file outside of your git repo in a folder called `instance` such that the `instance` folder would be parallel to your git repo.