# karabinar_setting
```json
{
    "description": "f + Spacebar -> japanese_eisuu, j + Spacebar -> japanese_kana",
    "manipulators": [
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "spacebar" },
                    { "key_code": "f" }
                ]
            },
            "parameters": { "basic.simultaneous_threshold_milliseconds": 100 },
            "to_if_alone": [{ "key_code": "japanese_eisuu" }],
            "type": "basic"
        },
        {
            "from": {
                "modifiers": { "optional": ["any"] },
                "simultaneous": [
                    { "key_code": "spacebar" },
                    { "key_code": "j" }
                ]
            },
            "parameters": { "basic.simultaneous_threshold_milliseconds": 100 },
            "to_if_alone": [{ "key_code": "japanese_kana" }],
            "type": "basic"
        }
    ]
}

```
