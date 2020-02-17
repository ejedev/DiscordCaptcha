# DiscordCaptcha
A Discord bot that requires users to answer a captcha to participate in your server.

# Requirements
Python module requirements available in `requirements.txt`

Tested with Python 3.7 on Ubuntu 18.04.3

# Setup Instructions
- Install the required modules from `requirements.txt`
- Create a new application at https://discordapp.com/developers/applications
- Turn it into a bot. Copy the token and put it on line 66 of `DiscordCaptcha.py`
- On the developer portal, Select "OAuth2"
- Select the "bot" checkmark and then "Manage "Roles"
- Copy the generated link and paste it in your browser. Select the server to add it to.
- Go to your server settings and find roles. Move the bot role above all user roles.
- Create your limited role and ensure that it is below the bot's role.
- Copy the limited role's ID and put it on line 11 of `DiscordCaptcha.py`
- Copy your server's ID and put it on line 13 of `DiscordCaptcha.py`
- Run `DiscordCaptcha.py`

# Optional Config
Feel free to modify anything in `CaptchaCreator.py` to change things like captcha length.

# Known Issues
- Creates a random captcha for some reason when the program first runs.
- I have no idea what happens if a user has DM's disabled

# Planned Features
- Handling for user having DM's turned off.
- Support for both Linux and Windows.
