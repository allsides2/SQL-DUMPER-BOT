# SQL Bot

## Introduction

This SQL bot is designed to automate the process of dumping SQL databases and sending the dumps to a Discord webhook. It provides functionality to schedule automatic dumps at specified intervals and sends the dumps to a configured Discord webhook.

## Features

- Automated SQL database dumps at specified intervals.
- Sends dumps to a Discord webhook for monitoring or backup purposes.
- Supports gzip compression for efficient file transfer.
- Easy configuration via a JSON configuration file.

## Setup

1. Clone this repository to your local machine or download the script files directly.

git clone https://github.com/allsides2/SQL-DUMPER-BOT.git

2. Install the required dependencies using npm:

npm install

3. Configure the bot by editing the `config/config.json` file:
- Specify the Discord webhook URL.
- Provide database connection details (host, database, user, password).
- Adjust the cooldown period for automatic dumps (in minutes).

## Usage

1. Start the bot by running the main script:


2. The bot will automatically dump the configured SQL database at the specified intervals.
3. Dumps will be sent to the configured Discord webhook for monitoring or backup purposes.
4. Monitor bot activity and dump notifications in the configured Discord channel.

## Customization

You can customize the bot behavior by adjusting the following settings in the `config/config.json` file:

- `webhook`: Discord webhook URL for sending dump notifications.
- `dump`: Configuration object containing database connection details and dump settings.
- `host`: SQL database host.
- `database`: SQL database name.
- `user`: SQL database user.
- `password`: SQL database password.
- `cooldown`: Cooldown period for automatic dumps (in minutes).

## Troubleshooting

- If the bot encounters errors or fails to connect to the database, check the configuration settings in `config/config.json`.
- Ensure that the Discord webhook URL is correct and the bot has permission to send messages to the specified channel.

## Contributing

Contributions are welcome! If you have any suggestions, improvements, or encounter any issues, feel free to open an issue or submit a pull request.
