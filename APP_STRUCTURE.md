# CLI App Directory structure

## Default App structure

Default script config setting:

```php
'cmd_dir'         => __DIR__ . '/app/Cmd',
'cmd_namespace'   => '',
```

Commands like ``` {script} {command} {subcommand or blank} ``` will execute the controller in the {cmd_dir}/{command}/ directory

### Default App Command

./{script} help will display help functions and the options available

## Namespaced App structure

Namespaced apps allow you to have multiple scripts and their own set of commands
e.g. ftp script will have it's own set of commands

```php
'cmd_dir'         => __DIR__ . '/app/Cmd/Ftp',
'cmd_namespace'   => 'Ftp',
```

Commands like ``` {script} ftp {command} {subcommand or blank} ``` will execute the controller in the {cmd_dir}/ftp/{command}/ directory

### Namespaced Help Command

./{script} ftp help will display help functions and the options available
