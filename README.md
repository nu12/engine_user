# EngineUser

Use EngineUser to study Engine development to Rails apps. Do not use in production.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'engine_user', :github => "nu12/engine_user"
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install engine_user

## Usage

Run `$ rails db:migrate` to run the migration within this gem.

In config/routes.rb:

```
mount EngineUser::Engine => ""
```

Access EngineUser resources from the browser normally (i.e: /users).


## Development

Caviats:
* Controllers must be in the engine scope, i.e: app/controllers/engine_user/user_controller.rb
* Views must be in the engine scope, i.e: app/views/engine_user/layouts/application.html.rb

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/nu12/engine_user.

## License

The gem is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).
