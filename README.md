# py_nmap_with_https_detect
> python-nmap lib default detect protocol https as http, it's not convenient.<br>
> the code add https protcol detection.<br><br>
## How to use?
### The usage is similar to original python-nmap lib,but just a little different in https detection.
```
p = scan_result['scan']['127.0.0.1']['tcp']['443']
if p['name'] == 'http' and p['tunnel'] == 'ssl':
  service = 'https'
elif p['name'] == 'ssl' and p['tunnel'] == 'ssl':
  service = 'https'
```
