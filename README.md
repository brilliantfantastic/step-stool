step-stool
==========
***

## DESCRIPTION

Custom Rails generator for creating applications with known-good gems, and common features with wrapping tests.

## AUTHENTICATION

```
Would you like to add authentication (using Sorcery)?
1. Yes
2. No
```

Selecting Yes will perform the following:

```
gem 'sorcery'
```

```
bundle install
```

```
rails generate sorcery:install
```

```
rake db:migrate
```

```
describe User do
  describe '.authenticate' do
    it 'returns the user if the username and password match' do
    end
  end
end
```

```
bundle exec rspec spec/models/user_spec.rb
```

```
Are you going to provide reset password functionality?
1. Yes
2. No
```

```
config.user_config do |user|
  user.reset_password_mailer = UserMailer
end
```
