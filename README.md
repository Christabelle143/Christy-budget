

<a name="readme-top"></a>


# 📗 Table of Contents

- [📖 About the Project](#about-project)
  - [🛠 Built With](#built-with)
    - [Tech Stack](#tech-stack)
  - [🚀 Live Demo](#live-demo)
- [💻 Getting Started](#getting-started)
  - [Setup](#setup)
  - [Prerequisites](#prerequisites)
  - [Install](#install)
  - [Usage](#usage)
  - [Run tests](#run-tests)
  - [Deployment](#triangular_flag_on_post-deployment)
- [👥 Authors](#authors)
- [🔭 Future Features](#future-features)
- [🤝 Contributing](#contributing)
- [⭐️ Show your support](#support)
- [🙏 Acknowledgements](#acknowledgements)
- [📝 License](#license)

# 📖 [Budget App] <a name="about-project"></a>

> Budget app is a mobile web application that allow users to manage their budget.

## 🛠 Built With <a name="built-with"></a>
- HTML & CSS
- Bootstrap
- JavaScript
- Ruby
- Ruby on Rails
- Rubocop
- Rspec
- Postgresql

### Tech Stack <a name="tech-stack"></a>

<details>
  <summary>Client</summary>
  <ul>
    <li><a href="https://www.ruby-lang.org/en/documentation/">Ruby</a></li>
  </ul>
</details>

<details>
  <summary>Server</summary>
  <ul>
    <li><a href="https://guides.rubyonrails.org/">Ruby on Rails</a></li>
  </ul>
</details>

<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.postgresql.org/">PostgreSQL</a></li>
  </ul>
</details>

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🚀 Live Demo <a name="live-demo"></a>

- [Live Demo Link](soon!!)

## 🚀 Video Presentation <a name="live-demo"></a>

- [Video Link](https://www.loom.com/share/c1ac0cf5489e4626922b2fa4a60ebc55)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 💻 Getting Started <a name="getting-started"></a>

## Getting Started

To get a local copy for this project and running follow these simple example steps.

### Prerequisites

- You need to have git installed in your machine.
- Install a recent version of Postgres.
- Already install Rails


## Setup

## Setting Up PostgreSQL

- The postgres installation doesn't setup a user for you, so you'll need to follow these steps to create a user with permission to create databases

```bash
$  sudo -u postgres createuser blog-app -s
```

### Creating the Budgy-Budget application

- To create project with PostgreSQL database 

```bash
$   rails new Christy-Budget --database=postgresql  #or

$   cd Rails-capstone-Budget-app # Move into the application directory
```


### Clone this repository

```bash
$ git clone git@github.com:Christabelle143/Christy-budget.git
$ cd Christy-Budget
```

### Create the database

```bash
$   rails db:create   # or
$   rake db:create
```

### Install linter and 

- Rubocop gem

```bash
$  bundle init
$  bundle install
```
- Stylelint package

```bash
$  npm init -y
$  npm install
$  npm install --save-dev stylelint@13.x stylelint-scss@3.x stylelint-config-standard@21.x stylelint-csstree-validator@1.x

```

- Run linter

```bash
$  rubocop .
$  npx stylelint "**/*.{css,scss}" 
```

- In auto-correct mode, RuboCop will try to automatically fix offenses:

```bash
$  rubocop -A # or
$  rubocop --auto-correct-all
$  npx stylelint "**/*.{css,scss}" --fix 
```


### Starting up the Web Server

```bash
$   rails s # or
$   rails server # or
$   rails server -p3001
```

- To restart the server

```bash
$  sudo service postgresql restart 
$  rails db:reset #to clean the database                                                                    
```

#### Listing Existing Routes

- You can now visit `http://localhost:3000` to view your new website!

 You can also execute the `rails routes` command in your terminal to produce the same output.


#### Generate rspec

- At the first you need to include those lines in your Gemfile

```bash
  gem 'rails-controller-testing'
  gem 'rspec-rails'
```

#### Install RSpec

```bash
$  rails generate rspec:install
```
- This should generate some files that you will need to run your tests and should give us a Controller and a View

- Then run:

```bash
$  rspec spec     # to test if your tests are passed
```

#### Generate MVC with scaffold

```bash
  $  rails g scaffold category name user:belongs_to
  $  rails g scaffold records name amount:decimal user:belongs_to 
  $  rails g scaffold category_records user:belongs_to
  $  rails g scaffold category_records category:belongs_to record:belongs_to
```

#### Generate Schema

- To push the Migration into the database

```bash
  $   rails db:migrate
```
- We use the seeds.rb file to records in the database
- To drop, create a table and to migrate and send the seed into the database:

```bash
  $   rails db:drop db:create db:migrate db:seed  
```

- To check available routes

```bash
  $   rails routes  
```

#### Run Capybara

```bash
$  bundle exec rspec ./spec/features/
```

#### Run spec

```bash
$  bundle exec rspec ./spec/models/
```


## 👥 Author <a name="authors"></a>

👤 ## Author

👤 **Youta Christabelle**

- GitHub: [Christabelle143](https://github.com/Christabelle143)
- Twitter: [@christabelleyo](https://twitter.com/christabelleyo)
- LinkedIn: [YoutaChristabelle](https://linkedin.com/in/YoutaChristabelle)
<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🔭 Future Features <a name="features"></a>
- Add a delete button to remove a category
- Add an edit button to edit the transactions

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🤝 Contributing <a name="contributing"></a>

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](https://github.com/Christabelle143/Christy-budget/issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## ⭐️ Show your support <a name="support"></a>

Give a ⭐️ if you like this project!

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 🙏 Acknowledgments <a name="acknowledgements"></a>

- Original design idea by [Gregoire Vella on Behance](https://www.behance.net/gregoirevella)
- Hat tip to anyone whose code was used

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## 📝 License <a name="license"></a>

This project is [MIT](./MIT.md) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>
