# CVE-2024-20767

### [CVE-2024-20767](https://nvd.nist.gov/vuln/detail/CVE-2024-20767) - Arbitrary file system read using an Improper Access Control vulnerability in Adobe ColdFusion

- Please refer to **ma4ter** blogpost for more information: [Adobe ColdFusion任意文件读取漏洞CVE-2024-20767分析](https://jeva.cc/2973.html)

![adobecoldfusionlogo](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEifs-eKZwEeCs01XEwWXs4KI4C-oz4drQ5UWGtBjFnbaeA2FQL3Gz9HoxifqYA2wXAN-FikPbNSJN4QqpHp0UG0zSSW7vpc4M1ss9gbkj8Nf6KjaDI7692QF5kol_8mpsghR8wkneLfCSEZarLq1JlINquinyxt6Bl8UMV-BkjY2UN1dyHiJvPBmHePvgRf/s728-rw-e30/cf.jpg)

*Products and Versions affected:*


| Product  | Affected Versions |
| :--------| :---------------- |
| ColdFusion 2023 | Update 6 and earlier versions |
| ColdFusion 2021 | Update 12 and earlier versions |

- **CVSS:** 8.2
- **Actively Exploited:** NO
- **Patch:** [YES](https://helpx.adobe.com/security/products/coldfusion/apsb24-14.html)
- **Mitigation:** NO

# Lab

You can deploy a ColdFusion server with a Free Trial from Adobe:

- [Download ColdFusion](https://helpx.adobe.com/coldfusion/kb/coldfusion-downloads.html#download0)

# Help

```
usage: CVE-2024-20767.py [-h] -t TARGET [-p PORT] -c COMMAND

options:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        Target Adobe ColdFusion Server URL
  -p PORT, --port PORT  Target Adobe ColdFusion Server Port, by default we use the 8500 Port
  -c COMMAND, --command COMMAND
                        Path to read file
```


**Example:** 

```
python CVE-2024-20767.py -t http://192.168.124.203 -p 8500 -c Windows/ServerStandardEval.xml
```

# References

- [Adobe ColdFusion任意文件读取漏洞CVE-2024-20767分析](https://jeva.cc/2973.html)
- [CVE-2024-20767: Critical Adobe ColdFusion Flaw Exposes Sensitive Files, PoC Published](https://securityonline.info/cve-2024-20767-critical-adobe-coldfusion-flaw-exposes-sensitive-files-poc-published/)
- [Security updates available for Adobe ColdFusion | APSB24-14](https://helpx.adobe.com/security/products/coldfusion/apsb24-14.html)
