# RailsCasts Example Application

Run these commands to try it out.

```
bundle
rake db:setup
rails s
```

Requires Ruby 1.9.2 or later to run.



# RailsCasts Episode #360: Facebook Authentication

http://railscasts.com/episodes/360-facebook-authentication

Requires Ruby 1.9.2 or higher.


### Commands used in this episode

```
rails g model user provider uid name oauth_token oauth_expires_at:datetime
rake db:migrate
```



# RailsCasts Episode #361: Facebook Graph API

http://railscasts.com/episodes/361-facebook-graph-api

Requires Ruby 1.9.2 or higher.


### Commands used in Rails console

```
u = User.first
u.facebook.get_object("me")
u.facebook.get_connection("me", "television")
u.facebook.get_object("22934684677")
u.facebook.get_object("TheBigBangTheory")
u.facebook.put_wall_post("testing")
u.facebook.get_connection("me", "permissions")

u = User.last
u.facebook.get_connection("me", "permissions")
u.facebook.put_wall_post("testing")
u.facebook.fql_query("select pic from page where username='amazon' or username='google'")
```



# RailsCasts Episode #363: Facebook Open Graph

http://railscasts.com/episodes/363-facebook-open-graph

Requires Ruby 1.9.2 or higher.

### Commands used in episode

```
gem install localtunnel
rbenv rehash
localtunnel -k ~/.ssh/id_rsa.pub 3000
rails g delayed_job:active_record
rake db:migrate
rake jobs:work
```

### Commands used in console

```ruby
u = User.last
u.facebook.put_connection("me", "cinematron:review", movie: "http://samples.ogp.me/457069940972565")
```
