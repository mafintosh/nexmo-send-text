# nexmo-send-text

Send sms texts from the command line using nexmo and bash

One line install

	curl -fs https://raw.github.com/mafintosh/nexmo-send-text/master/install | bash && . $(bashkit rc)

After installation you should be able to run

	send-text # prints out a help

## Usage

You will need an account on [nexmo.com](https://nexmo.com) as well to get an api key and api secret.
To send a `hello world` message do:

	send-text hello world --to 4512345678 --key your_api_key --secret your_api_secret

Where `4512345678` is your telephone number. To set these options as default values do

	send-text --to 4512345678 --key your_api_key --secret your_api_secret --defaults

Thats it! You are now ready to go.

This script can be really useful if you are running a script that takes a long time to finish
and you want to get notified when its done. Using `send-text` just do

	long-running-command; send-text the script is done

## License

MIT
