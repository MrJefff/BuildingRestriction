**BuildingRestriction** will automatically remove building blocks (when placed) that have reached the configured maximum building height, when built in water, or if the maximum number of foundations has been reached. Each restriction can be enabled/disabled via the configuration file.

**Note:** The water limit is calculated based on the bottom point of the building block; ex. foundations it would be the bottom of the posts.

## Permissions

- **buildingrestriction.bypass** -- excludes player from restrictions

## Configuration

You can configure the settings in the BuildingRestriction.json file under the oxide/config directory.
```json
{
  "Restrict build height (true/false)": true,
  "Maximum build height": 5,
  "Restrict foundations (true/false)": true,
  "Maximum foundations": 16,
  "Maximum triangle foundations": 24,
  "Restrict water depth (true/false)": true,
  "Maximum water depth": 0.1,
  "Refund resources when restricted": true
}
```

## Localization

The default messages are in the BuildingRestriction.json under the oxide/lang directory. To add support for another language, create a new language folder (ex. de for German) if not already created, copy the default language file to the new folder, and then customize the messages.
```json
{
  "MaxBuildHeight": "You have reached the max building height! ({0} building blocks)",
  "MaxFoundations": "You have reached the max foundations allowed! ({0} foundations)",
  "MaxTriFoundations": "You have reached the max triangle foundations allowed! ({0} foundations)",
  "MaxWaterDepth": "You are not allowed to build in water!"
}
```

## Credits
- **Jakkee**, for the original version of this plugin.
