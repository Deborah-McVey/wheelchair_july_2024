install rspec first

rails g scaffold Post description:text location:string

rails g migration add_status_to_posts status:string

after fully installing devise,

rails g migration add_user_id_to_posts user_id:integer:index