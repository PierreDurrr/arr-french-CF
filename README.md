# arr_french-CF
Collection of french custom formats available in .json format, ready to import to radarr and sonarr (v4)

**Example**

```json
{
  "name": "Special Edition",
  "includeCustomFormatWhenRenaming": false,
  "specifications": [
    {
      "name": "Special Edition",
      "implementation": "ReleaseTitleSpecification",
      "negate": false,
      "required": true,
      "fields": {
        "value": "(?<!^)\\b(extended|uncut|director|special|unrated|uncensored|cut|version|edition)(\\b|\\d)"
      }
    },
    {
      "name": "Not Theatrical ",
      "implementation": "ReleaseTitleSpecification",
      "negate": true,
      "required": true,
      "fields": {
        "value": "Theatrical"
      }
    }
  ]
}
```
