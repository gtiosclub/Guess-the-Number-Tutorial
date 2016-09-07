# How to port this to Legacy GT iOS Website

1. Move all of the contents in `assets/guessthenumber/*.png` to `app/assets/images/guessthenumber/` in the rails-site
2. `rm -rf public` when in the root directory of the rails-site
3. `rake assets:precompile` to compile the assets
4. `rails s` to run the server on `localhost:3000`
5. To push to heroku, git add, git commit, and then `git push heroku master` if you have permission.
