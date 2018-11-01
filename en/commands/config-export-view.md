# config:export:view
Export a view in YAML format inside a provided module to reuse in another website.

**Usage:**
```
drupal config:export:view [arguments] [options]
cev
```

## Available options
Option | Details
-------|-------------
--module | The Module name.
--optional-config | Export view as an optional YAML configuration in your module
--include-module-dependencies | Include module dependencies in module info YAML file

## Available arguments
Argument | Details
---------|-------------
view-id | View ID

## Examples
* Perform a simple export.
```
drupal config:export:view viewid
```
* Export as optional config for the provided module.
```
drupal config:export:view viewid \
  --module="modulename" \
  --optional-config \
  --include-module-dependencies
```
* Export as config for the provided module, updating the module's info.yml
with any module dependencies from the view.
```
drupal config:export:view viewid \
  --module="modulename" \
  --optional-config \
  --include-module-dependencies
```
