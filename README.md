## Ruby on Rails 7 docker template with mysql

1. First clone the project
```
$ git clone https://github.com/Mashpy/rails-7-docker-template-with-mysql.git
```

2. Rename the project name as your wish
```
$ mv rails-7-docker-template-with-mysql your_project_name
```

3. Change directory -
```
$ cd your_project_name
```

4. Update your rails version on the Gemfile -
```
source 'https://rubygems.org'
gem 'rails', '7.0.3'
```

5. Update Ruby version on Dockerfile -
```
FROM  ruby:3.1.2-slim
```

6. Now install new rails app -
```
$ docker-compose run app rails new . --force --database=mysql --skip-bundle
```
7. Build the docker image -
```
$ docker-compose build
```
8. Run - 
```
$ docker-compose up
```

9. Browse http://localhost:3000
![Ruby on rails 7.0.3 docker with mysql](https://i.ibb.co/Z19FNSJ/Screenshot-2022-07-30-at-9-11-24-PM.png) 
