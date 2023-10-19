# macOS PHP version switcher script

## Description and usage

It's a simple script for macOS which assumes you have PHP versions 5.6, 7.1, 7.2, 7.3, 7.4, 8.0 installed (for example, from this tap: [shivammathur/php](https://github.com/shivammathur/homebrew-php)) using Homebrew (the list of versions can be changed in the script).

You can use it like this: `./phpvm.sh 7.4`, and it would switch you to PHP v7.4 (if it's installed and is in your list). If you're already on this version, script would return "PHP v7.4 is already selected!" and will do nothing. If 7.4 isn't in the list of the available versions in the script, it would return "Error: PHP v1.5 is not available! (available versions: 5.6, 7.1, 7.2, 7.3, 7.4, 8.0)".

You can copy it to your `/usr/local/bin` directory: `sudo cp ./phpvm.sh /usr/local/bin/phpvm && sudo chmod +x /usr/local/bin/phpvm`. Then you'll be able to run it from any other directory, just like this: `phpvm 7.1`.
