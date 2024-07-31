This is a full stack application in Ruby on Rails. 

If someone has a wheelchair they don't need anymore and want to offer it up to someone for free to come pick up.

A person will be able to make a post with a photo upload, description, location, and status (available, pending, sold). Other people can comment. The original publisher can also comment.

Rails version: 7.1.3.4
Ruby version: ruby 3.2.2 (2023-03-30 revision e51014f9c0) [x86_64-linux]

rails g scaffold Post description:text location:string

gems necessary:

rspec for tests

https://medium.com/@anaharris/how-to-add-image-upload-functionality-to-your-rails-app-9f7fc3f3d042

active_storage for photos

rails active_storage:install

devise for login functionality

migration to add user to post schema

rails g migration add_user_id_to_posts user_id:integer:index

migration to add status to posts

rails g migration add_status_to_posts status:string

set up enums with status options (default is available, then pending, and sold)

The date posted will show.

There will be a home page with navbar with options to login/signup. Once logged in: sign out, edit profile. 