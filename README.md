# fika-deployer script

![fika-deployer](https://dl.dropboxusercontent.com/u/697441/fika-deployer.png)

Use is like this:

    ./deploy package.apk 1.0.1 "Updated misc thing" team,xxx

Settings.

    Create file ~/.fika_developer

With some tokens. Like this:

    {
    "hockeyapp_token": "<put hockey app token here>",
    "hc_room_id": "<hipchat room token>",
    "hc_api_key": "<hipchat api key"
    }

You can find your HipChat [tokens here](https://www.hipchat.com/account/api). And HockeyApp auth [tokens here](https://rink.hockeyapp.net/manage/auth_tokens).


## Workflow

- Detect package "OS"
- Determine version
- Loads configuration
- Uploads package to [HockeyApp](http://hockeyapp.net)
- On success report new release information to [HipChat](https://www.hipchat.com/)
- Add Git Tags and report them to [GitHub](https://github.com) - *(in progress)*

## Ruby 1.8

    ruby --version
    sudo gem install json
