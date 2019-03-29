# python-nmap_with_https_detect
> python-nmap lib is a excellent lib for binding nmap. but it can't detect protocol https by default, it's not so convenient sometime.<br>
> this code add https protcol detection.<br><br>
## How to use?
### The usage is similar to original python-nmap lib,but just a little different in https detection.
```
    p = scan_result['scan']['127.0.0.1']['tcp']['443']
    if p['name'] == 'http' and p['tunnel'] == 'ssl':
        service = 'https'
    elif p['name'] == 'ssl' and p['tunnel'] == 'ssl':
      service = 'https'
```
