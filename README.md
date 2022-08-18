# Rails deploy

Deploying a rails site to a server.

## Create a server(VM)

`brew install multipass`

`multipass launch --name rails-deploy jammy`

`multipass shell rails-deploy`

## Setup server

`sudo apt update`

Install ruby and dependencies 

`sudo apt install -y ruby ruby-dev build-essential`

`sudo apt install -y sqlite libsqlite3-dev`

`sudo gem install rails bundler`

## Create Rails site

`rails new blog`

## Run rails site

`cd blog`

`bin/rails server -b 0.0.0.0`

## Deploy rails site

## Verify rails site

`curl 192.168.64.2:3000`

## Cleanup



## Assumptions: 
* Write on Mac to deploy on Linux