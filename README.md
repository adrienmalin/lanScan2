# lanScan

Scan hosts with nmap and display results in webpage.

* Create a configuration yaml file in site/ subdirectory (see example below).
It may be generated by scanning a network with `init.sh`.
* Scan with `php scan_all.php` (use a cron task!).
* Open index.php to see results.

## Example 
```yaml
site:
  group1:
    host1.local: [ssh, http]
    host2.local: [ftp, https, 5432]
  group2:
    host3: [ssh, ftp, 8006]
```

