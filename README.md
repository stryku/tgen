# Table generator
Generate markdown table from clipboard content.

Writes result to stdout and copies it to clipboard.

Example clipboard content:
```
aa :bb cc: :dd:
aaaaa bbbbbb ccccc ddddd
a b c d
```

Result:
```
|  aa   |   bb   |  cc   |  dd   |
|-------|--------|------:|:-----:|
| aaaaa | bbbbbb | ccccc | ddddd |
| a     | b      |     c |   d   |
```

# Requirements
pip3 install pyperclip pytablewriter
