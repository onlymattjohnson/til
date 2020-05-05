# Copy parent settings to child theme

You can copy over all the settings from a parent them to a child them using [WP CLI](https://developer.wordpress.org/cli/commands/option/) 
where 

- `{parent_theme_name}` --> The name of the your parent them

```bash
# save existing theme settings
wp option get theme_mods_{parent_theme_name} --format=json > theme_mods_{parent_theme_name}.txt

# load the saved settings into child theme
wp option update theme_mod_{parent_theme_name}-child --format=json < theme_mods_{parent_theme_name}.txt

# remove tmp text file
rm -rf theme_mods_{parent_theme_name}.txt
```