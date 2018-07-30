# Configure VS Code to work better

Configuration of the **VS Code** to work comfortably with **Python**.


## Snippets for Python

Do `Preferences -> User Snippets -> Python` to open `snippets/python.json` file and edit it.

```json
{
  "Print to console": {
    "prefix": "log",
    "body": [
      "from absl import logging",
      "logging.info('---> %s', $1)",
      "$2"
    ],
    "description": "Log output to console"
  },
  "Pretty print to console": {
    "prefix": "logpretty",
    "body": [
      "from absl import logging",
      "from json",
      "logging.info('---> %s', json.dumps($1, sort_keys=True, indent=2))",
      "$2"
    ],
    "description": "Log prettified output to console"
  }
}
```
