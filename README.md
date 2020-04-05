# Table generator
Generate markdown table from clipboard content.

Writes result to stdout and copies it to clipboard.

If `_` is used as header name, the header will be empty.

If value contains whitespaces, `|` should be used to separate all values in the row.

If there is no enough values in a row, empty values will be added.

Example clipboard content:
```
_ aa :bb cc: :dd:
----- aaaaa bbbbbb ccccc ddddd 
- a b c d
- | a || c | value with    whispaces 
- a 
```

Result:
```
|       |  aa   |   bb   |  cc   |           dd            |
|-------|-------|--------|------:|:-----------------------:|
| ----- | aaaaa | bbbbbb | ccccc |          ddddd          |
| -     | a     | b      |     c |            d            |
| -     | a     |        |     c | value with    whispaces |
| -     | a     |        |       |                         |
```

# Requirements
pip3 install pyperclip pytablewriter
