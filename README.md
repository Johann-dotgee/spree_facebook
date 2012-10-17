Spree Facebook (spree_facebook)
=============

Spree Facebook is a gem working with spree_profiles, spree_social and spree_social_products.
It allows you do make your spree website social by likable products, facebook authentication, etc.


Display
=======

If you want to test it, just visite the demo website/facebook app.

http://dotspree-facebook.srvdev02.dotgee.fr/products
http://apps.facebook.com/dotspree-facebook/

Installation
============
In your `Gemfile`:
```ruby
 gem 'spree_profiles', :git => 'https://github.com/Johann-dotgee/spree_profiles.git'
 gem 'spree_social_products', :git => 'https://github.com/Johann-dotgee/spree_social_products.git'
 gem 'spree_social', :git => 'https://github.com/spree/spree_social.git'
 gem 'spree_facebook', :git => 'https://github.com/Johann-dotgee/spree_facebook.git'
```

Then, just run
```bash
 bundle update
 bundle exec rails g spree_social:install
 bundle exec rails g spree_profiles:install
 bundle exec rails g spree_social_products:install
 rake db:migrate
```

Configuration
=============

If you want the products to be likable only in a facebook app, just go on http://your-website.com/admon/social/edit and check the checkbox `Products likable only in the facebook app`.

If you want the user to be redirected on your website when he tries to look at a product, just set Spree::Config.direct_link to `true`.


Testing
-------

To do




Copyright (c) 2012 [dotgee], released under the New BSD License
