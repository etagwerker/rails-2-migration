!SLIDE full-page
# De Rails 2.3.x
# a Rails 3.0.6

!SLIDE bullets incremental full-page
# Pasos #

* Tests
* Instalar rails_upgrade
* rake rails:upgrade:check
* Solucionar Issues
* Correr Tests

!SLIDE full-page

# Tests #

![Why u no write tests](Y-U-NO-write-tests.jpg)


!SLIDE full-page

# Instalar rails_upgrade #

<code>
  script/plugin install git://github.com/rails/rails_upgrade.git
</code>

!SLIDE full-page

# Source #

[http://omgbloglol.com/post/353978923/the-path-to-rails-3-approaching-the-upgrade](http://omgbloglol.com/post/353978923/the-path-to-rails-3-approaching-the-upgrade)

!SLIDE full-page

# rake rails:upgrade:check

![Rake rails upgrade output](1.rake-rails-upgrade.png)

!SLIDE full-page

# rake rails:upgrade:gems

![Rake gems output with Gemfile content](2.rake-gems.png)

!SLIDE full-page

# rake rails:upgrade:routes

![Rake routes output with new routes content](3.rake-routes.png)

!SLIDE full-page

# find(:all) + find(:first) deprecated

![find(:all) and find(:first) are now deprecated](4.querying-changes.png)

!SLIDE full-page

# foo.find(:all) => foo.all

![A new way of querying is here](4.new-querying-mechanisms.png)

!SLIDE full-page

# cambios de constantes

![Constants moved to Rails class](5-deprecated-constants.png)

!SLIDE full-page

# nueva implementación de mailer

![Mailers no longer in app/models which was messy](6.new-mailer-implementation.png)

!SLIDE full-page

# app/mailers/my_mailer.rb

![Now mailers in app/models](7.new-mailers-location.png)

!SLIDE full-page

# gem install rails

![gem install rails 3 that you want](8-install0-rails-3.png)

!SLIDE full-page

# como dice borat

![Follow Borat's advice and create a rails on a rails project](ahh-u-wanna-Rails-3-ahh-yess-rails-new-foo.jpg)

!SLIDE full-page

# overwrite paso por paso

![This will override some shit. Be careful and create a separate branch](9-create-rails-on-top-of-rails.png)

!SLIDE full-page

# rails server, y..?

![This will probably not work](11-try-to-run-rails-server.png)

!SLIDE full-page

# encoding: utf-8

![You might run with encodings problem. It's 1.9 after all](10-check-encodings-problem.png)

!SLIDE full-page

# missing mysql2? 

![You will need to fix things like this](12-mysql2-problem.png)

!SLIDE full-page

# gem 'mysql2'

![But mysql2 was necessary](13-a-gemfile-with-mysql2.png)


!SLIDE bullets incremental full-page

# Test checklist: #

* rails server
* Correr tests
* Actualizar gems
* Correr tests

!SLIDE full-page

# Muchas gracias!

<code>http://github.com/etagwerker</code>

<code>http://twitter.com/_nesto</code>