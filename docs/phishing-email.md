## 🎣 Phishing & Email Investigation

[← Back to Index](../README.md)

### Email Breach and Reputation
- [Have I Been Pwned](https://haveibeenpwned.com/) — Search if an email appears in known data breaches  
- [DeHashed](https://dehashed.com/) — Breach and credential search  
- [EmailRep.io](https://emailrep.io/) — Email reputation and risk scoring  
- [Hunter.io](https://hunter.io/) — Discover corporate email patterns and addresses  

### Email Analysis
- [MX Toolbox](https://mxtoolbox.com/EmailHeaders.aspx) — Email header analyzer and MX tools  
- [mailtester.com](http://mailtester.com/) — Check if an email address is valid and deliverable  
- [VerifyEmail](https://tools.verifyemailaddress.io/) — Verify the validity of an email address  

### Breach hunting & Email Recon
- [h8mail](https://github.com/khast3x/h8mail) — Email OSINT & breach-hunting tool (local breaches + commercial APIs)

	h8mail searches local breach collections and a range of breach/recon APIs to find leaked credentials and related emails. It supports bulk files, gzip archives, multiprocessing, CSV/JSON output and optional API integrations (HaveIBeenPwned, Dehashed, Snusbase, Hunter, Leak-Lookup, IntelX, etc.).

	Installation:

	```powershell
	pip install h8mail
	```

	Quick examples:

	```powershell
	# single target
	h8mail -t target@example.com

	# list of targets -> CSV, using config for API keys
	h8mail -t targets.txt -c config.ini -o pwned_targets.csv

	# use a local Breach Compilation folder (fast local scans)
	h8mail -t targets.txt -bc "C:\path\to\BreachCompilation" -sk
	```

	Notes: some API lookups require API keys; use `--gen-config` to create a template config file. See the h8mail repo for advanced options and examples.

### URL and Phishing Kit Analysis
- [urlscan.io](https://urlscan.io/) — Sandbox and visualize web requests from a URL  
- [URLquery](http://urlquery.net) — Analyze suspicious URLs and detect malicious behavior  
- [PhishTank](https://phishtank.org/) — Community-driven phishing URL database  
- [OpenPhish](https://openphish.com/) — Automated phishing feed  
- [StalkPhish](https://github.com/t4d/StalkPhish) — Identify phishing kits and reused infrastructures  

### IOC and Threat Intelligence Integration
- [Maltiverse](https://maltiverse.com/search) — IOC enrichment and threat intelligence search  
- [ThreatMiner](https://www.threatminer.org/) — IOC and malware sample data mining  
- [ThreatCrowd](https://threatcrowd.org/) — Investigate domains, IPs, and emails via visual graphs  
