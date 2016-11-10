# How to port this to Legacy GT iOS Website

1. Move all of the contents in `assets/guessthenumber/*.png` to `app/assets/images/guessthenumber/` in the rails-site
2. Move all of the tutorials .md files (part*.md) to `app/assets/tutorials/guessthenumber/`
3. `rm -rf public` when in the root directory of the rails-site
4. `rake assets:precompile` to compile the assets
5. `rails s` to run the server on `localhost:3000`
6. To push to heroku, git add, git commit, and then `git push heroku master` if you have permission.

# Tutorial

##### [Part 1: Getting Started](part1.md)
##### [Part 2: Setting up your View](part2.md)
##### [Part 3: Generate Random Numbers](part3.md)
##### [Part 4: Writing the Game Logic](part4.md)
##### [Part 5: Adding Alerts!](part5.md)
##### [Part 6: Finishing Up (Github)](part6.md)
