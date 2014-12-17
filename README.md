# HAL42

The IRC bot for the **Equilibre** organization.

## Installation

```bash
npm install
mv config.json.default config.json
```

Then, you have to modify the `config.json` file

## Usage

This is an example of a configuration file:

```json
{
    "name": "HAL42",
    "channels": ["#equilibre", "#4242"],
    "primaryChan": "#4242", // the channel to forward master's messages
	"customParams": { // this parameters will be used at the connection
		"userName": "HAL42",
		"realName": "HAL42",
		"password": "",
		"sasl": true
    },
    "server": "irc.freenode.net",
    "master": ["Alpha14", "Emeraude"], // the bot will forward their private messages
    "react": { // the bot will response if one on the words "bocal", "php" or "ubuntu" is said
		"bocal": "https://i.imgur.com/Qg1SrLe.png",
		"php": "https://i.imgur.com/vlpkkUM.jpg"
		"ubuntu": "http://cdn.meme.am/instances/54738442.jpg"
    },
    "talkAboutMe": { // the bot will response if one on the words "merci" or "bot", and the name of the bot is said
		"merci": "de rien :)",
		"bot": "Je ne suis pas un bot !"
    },
    "history": true // write all the messages said in stdout
}
```

### Contributors

Alpha14  
Emeraude
