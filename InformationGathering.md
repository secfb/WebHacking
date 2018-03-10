# Information Gathering


### Subdomain Discovery for choosing a target


###### 1\. Sublist3r - Scanning for subdomains
```
sublist3r -d <domain>
```


###### 2\. Striker - Offensive information and vulnerability scanner
Scanning for services running on ports 
```
cd Striker && python striker.py
```



##### Others


###### 1\. Cloudfail - Utilize misconfigured DNS and old database records to find hidden IP's behind the CloudFlare network.
To run a scan against a target:
```
cd CloudFail && python3 cloudfail.py --target <domain>
```


### Target specifiec 

###### 2\. Nmap Vulners - NSE script based on Vulners.com API 
Scanning for services running on ports 
```
nmap -p-  -sV  --script vulners <domain>
```


###### 2\. Nikto - Web server scanner
Scan for configurations ...
```
nikto -h <domain> -C all
```

![Recon](https://github.com/Zawadidone/Hacking/blob/master/images/Recon.jpg?raw=true)