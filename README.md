## ActiveRecord basics boilerplate

This is a minimalist implementation of ActiveRecord with one `Restaurant` model of my first live-code as a student of the @LeWagon working with Sinatra.

- clone the repo
- run `rake db:create` to create your db
- run your migrations with `rake db:migrate`

Now you can play with the `Restaurant` model:

```bash
$ irb
irb> load "config/application.rb"
irb> restaurant = Restaurant.new(name: "Pitaya", address: "42 Rue Saint-Rémi, 33000 Bordeaux")
irb> restaurant.id
     # => nil
irb> restaurant.save
irb> restaurant.id
     # => 1
```

To launch a Sinatra server just run `ruby app.rb` and open a web browser at [http://localhost:4567](http://localhost:4567)

Enjoy!
