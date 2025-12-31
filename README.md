# CLI App Template

Template for cli apps using minicli

## Script file

./minicli is the base file that the app will run through, rename it what you'd
like your base command to be called, make file executable using chmod

``` bash
chmod +x {script}
```

## Help Command

./{script} help will display help functions and the options available

## .env Environment Variables

Set up your Environment by setting Variables in the .env file
Look at the .env-example file for variables that should be set

## install.sh

Set up server environment by running this shell script as root

## Setup PHP CLI environment

1. Run ``` ln -s /usr/bin/php /usr/bin/phpcli ``` for default php
OR
 Run ``` ln -s /usr/bin/php72 /usr/bin/phpcli ``` for php 7.2

2. Then in the scripts update ``` /usr/php/cli ``` to ``` /usr/bin/phpcli ```
