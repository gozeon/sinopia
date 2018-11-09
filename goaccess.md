# base config
```
log-format %h %^[%d:%t %^] "%r" %s %b "%R" "%u" %T
date-format %d/%b/%Y
time-format %H:%M:%S
```

# terminal

```
goaccess -f <path>/access.log -c
```

# generator html

```
goaccess --no-global-config --log-format='%h %^[%d:%t %^] "%r" %s %b "%R" "%u" %T' --date-format=%d/%b/%Y --time-format=%H:%M:%S -f <path>/access.log -o report.html
```
