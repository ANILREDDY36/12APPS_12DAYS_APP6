# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

steps to follow:
1) rails g scaffold todo_list title:string description:text
	rails db:migrate
2) rails g model todo_item content:string todo_list:references
	rails db:migrate
3) rails g controller todo_items
4) rails g migration add_completed_at_to_todo_items completed_at:datetime
	rails db:migrate