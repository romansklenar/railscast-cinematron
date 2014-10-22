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
