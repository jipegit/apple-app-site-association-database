# Apple app-site-association Database

This repository archives associations between Apple Team Identifiers, Bundle Identifiers and domain names. Such associations can be useful for macOS/iOS digital forensics investigations.

Data comes from app-site-association files available on Alexa TOP 100k websites. **Do not expect it to be exhaustive**. 

More information about app-site-association files can be found on [Apple Developer website](https://developer.apple.com/documentation/uikit/core_app/allowing_apps_and_websites_to_link_to_your_content/enabling_universal_links).

The JSON database format is described below:
```
[
    {
        team_id: [
            {
                "bundle_id": bundle_identifier,
                "domain": domain_name
            },
            ...
        ]
    },
    ...
]
```

Eg: for Facebook's Team ID "G2H69UVXYE":
```
[
    {
        "G2H69UVXYE": [
            {
                "app_id": "com.leaplock.ColorfulBalloonsDev",
                "domain": "facebook.com"
            },
            {
                "app_id": "com.leaplock.ColorfulBalloons",
                "domain": "facebook.com"
            },
            {
                "app_id": "com.leaplock.ColorfulBalloonsDev",
                "domain": "fb.com"
            },
            {
                "app_id": "com.leaplock.ColorfulBalloons",
                "domain": "fb.com"
            }
        ]
    }
]
```

# Contact

You can contact me on Twitter [@Jipe_](https://twitter.com/Jipe_)