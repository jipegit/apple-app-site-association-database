# Apple app-site-association Database

This repository archives associations between Apple Team IDs, websites and application IDs for (mobile) forensics and investigation purposes.

The JSON database format is described below:
```
[
	{
		"team_id": [
			{
				"app_id": "application_id",
				"domain": "domain_name"
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