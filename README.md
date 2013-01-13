# Feed aggregator for beerbloggers !

## What the f*&% is #beerblogging ?

It's a f*&%cking bet!

## Who are the Beerbloggers ?

* Victor Fontes - http://victorfontes.com/ - http://victorfontes.com/feed/
* Pedro Marins - http://pedromarins.com/ - http://pedromarins.com/feed/
* Arlindo Pereira - http://nighto.net/ - http://nighto.net/feed/
* Tiago Veloso - http://tiagoveloso.com/ - http://tiagoveloso.com/feed/
* Felipe Arruda - http://www.arruda.blog.br/ - http://www.arruda.blog.br/?feed=rss2
* Zeno Rocha - http://blog.zenorocha.com/ - http://feeds.feedburner.com/zenorocha
* Thiago Belem - http://blog.thiagobelem.net/ - http://blog.thiagobelem.net/feed/
* Thiago Avelino - http://avelino.us/ - http://feeds.feedburner.com/pyavelino

If you are beerblogging, add yourself to members.yaml and make a pull request

## Let's talk about code...

* `Python <http://python.org/>`_ programing language
* `Flask <http://flask.pocoo.org/>`_ microframework for web
* `Feed Parser <http://www.feedparser.org/>`_ library

## Let's install the f*&%cking thing

* To install it, first you need to clone this repository
* Then install all requirements, using 'beerblogging/beerblogger/etc/requirements.txt'
* Run "manage.py create_db" to create the DB
* Run "manage.py fetch_posts" to populate the DB
* Run "manage.py run" to run server in localhost:5000

## Deploying

* To deploy on Heroku:
* heroku create
* heroku addons:add heroku-postgresql:dev
* heroku pg:promote HEROKU_POSTGRESQL_COLOR_URL
* git push heroku master
* heroku run python manager.py create_db
* heroku run ./update_posts.sh
* 
**OBS:** The update_posts.sh should be runned everytime, to keep tracking new posts.
