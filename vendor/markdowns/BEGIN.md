install rspec first

factory_bot and faker for testing

most important for post is photo and description

also need location (city, state) and status (available, pending, sold)

easiest to start with description

rails g scaffold Post description:text

rails g migration add_status_to_posts status:string

after fully installing devise,

rails g migration add_user_id_to_posts user_id:integer:index