# twitter-notification-centre

Script to periodically run a twitter search and post notifications in Mac OS X notification centre.

![Exmaple in notification centre](https://raw.githubusercontent.com/rjlee/twitter-notification-centre/master/assets/example.png "")

It is designed to to run on your Mac and requires you to setup a twitter app that will search twitter using your credentials.  It uses the twitter gem https://github.com/sferik/twitter and instructions for setting up an app can be found in the README.

## Requires

* [Ruby](https://www.ruby-lang.org/en/)
* [Bundler](http://bundler.io/)

## Install

```
bundle install
ruby notify.rb --help

Usage: notify.rb [options]

        --search SEARCH              the search string to search twitter for
        --delay DELAY                the time in seconds between checking for updates
        --verbose                    displays verbose output
        --consumer-key KEY           the consumer key for the app
        --consumer-secret SECRET     the consumer secret for the app
        --access-token TOKEN         the access token for the user
        --access-token-secret SECRET the access token secret for the user
```

## Run

```
ruby notify_server.rb start -- --search "securitay" --delay 60 --consumer-key "app-key" \
--consumer-secret "app-secret" --access-token "your-token" -access-token-secret "your-secret"
```

## License

The software is made available under the Apache 2.0 license.  Any assets under the /assets directory are sourced from the web and as such their provenance is unknown.
