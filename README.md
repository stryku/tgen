# Table generator
Generate markdown table from clipboard content.

Writes result to stdout and copies it to clipboard.

If `_` is used as header name, the header will be empty.

Example clipboard content:
```
_ aa :bb cc: :dd:
----- aaaaa bbbbbb ccccc ddddd 
- a b c d
```

Result:
```
|       |  aa   |   bb   |  cc   |  dd   |
|-------|-------|--------|------:|:-----:|
| ----- | aaaaa | bbbbbb | ccccc | ddddd |
| -     | a     | b      |     c |   d   |
```

# Requirements
pip3 install pyperclip pytablewriter
