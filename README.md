# Online Shopping Mall

## Authors

- Tam Le
- Luis Del Mar
- Keaton Burleson

## How to Run

After downloading the artifact, please navigate into the artifact's directory.

1. Install Imagemagick (used for resizing product images)
   > Please visit https://imagemagick.org/script/download.php for more up-to-date information

    * macOS:
      ```shell
      brew install imagemagick && brew install ghostscript
      ```
    * [Windows](https://imagemagick.org/script/download.php#windows)
    * [Linux](https://imagemagick.org/script/download.php#linux)

2. Install Rubygem dependencies:

```shell
bundle install
```

3. Install Yarn dependencies:

```shell
yarn
```

4. Migrate database and seed data:

```shell
rails db:migrate:reset && rails db:seed
```

5. Run

```shell
rails s
```

**Note** if you are having trouble with styles not rendering in `development`, please open a new terminal window
inside the project root and run:
```shell
bin/webpack-dev-server
```

*Currently, we do not know why some machines have this issue and others do not*

## Live Demo

A live demo is available [here](https://pure-crag-94276.herokuapp.com/). As the app is 
hosted on Heroku, the application might take a minute or so to start up.

### Demonstration Accounts

After seeding the database, you should have the following accounts available:

|     Username    | Password | Abilities                                      |
|:---------------:|:--------:|------------------------------------------------|
| buyer@test.com  | password | Buy, review, and report sellers                |
| seller@test.com | password | List items, modify inventory, ship orders      |
| admin@test.com  | password | Disable seller accounts and view abuse reports |