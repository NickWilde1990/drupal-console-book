# config:export:single
Export a single configuration or a list of configurations as yml file(s).

**Usage:**
```
drupal config:export:single [options]
ces
```

## Available options
Option | Details
-------|-------------
--name | commands.config.export.single.options.name
--directory | commands.config.export.arguments.directory
--module | The Module name.
--include-dependencies | Export dependencies of the configuration as well.
--optional | Export config as an optional YAML configuration in your module
--remove-uuid | If set, the configuration will be exported without uuid key.
--remove-config-hash | If set, the configuration will be exported without the default site hash key.

## Examples
* Provide config settings name to be exported
```
drupal config:export:single \
  --name=config.settings.name
```
* Export with uuid and config hashes removed.
```
drupal config:export:single \
  --name=config.settings.name \
  --remove-uuid \
  --remove-config-hash
```
