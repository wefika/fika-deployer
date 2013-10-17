# fika-deployer script

Use is like this:

    ./deploy package.apk 1.0.1 "Updated misc thing" team,xxx

Settings.

    Create file ~/.fika_developer


## Workflow

- Detect package "OS"
- Determine version
- Loads configuration
- Uploads package to [HockeyApp](http://hockeyapp.net)
- On success report new release information to [HipChat](https://www.hipchat.com/)
- Add Git Tags and report them to [GitHub](https://github.com)

## Ruby 1.8

    ruby --version
    sudo gem install json
