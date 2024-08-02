def create
  @post = Post.find(params[:post_id])
  @comment = @post.comments.create(comment_params)
  @comment.user_id = current_user.id #or whatever is you session name
  if @comment.save
 
https://stackoverflow.com/questions/34757168/ruby-on-rails-adding-comments-to-post

https://dev.to/jkevinbaluyot/create-post-and-comment-in-ruby-on-rails-3d8c

https://github.com/jkevinbaluyot/PostAndComment

need post_id

post has_many comments

comment belongs_to post

