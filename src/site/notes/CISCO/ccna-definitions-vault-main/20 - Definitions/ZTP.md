---
{"dg-publish":true,"permalink":"/cisco/ccna-definitions-vault-main/20-definitions/ztp/","tags":["defs_ccna"]}
---

#### ZTP
- *Zero Touch Provisioning (ZTP)* is an automatic configuration protocol that allows [[CISCO/ccna-definitions-vault-main/20 - Definitions/Lightweight APs\|Lightweight APs]] to receive configurations from a [[CISCO/ccna-definitions-vault-main/20 - Definitions/WLC\|WLC]]
- There are several ways for a *Lightweight AP* to receive configuration instructions
	- [[CISCO/ccna-definitions-vault-main/20 - Definitions/DHCP\|DHCP]] - `option 43` gives the [[CISCO/ccna-definitions-vault-main/20 - Definitions/IPv4\|IP address]] of the WLC
		- Most commonly used method
	- [[CISCO/ccna-definitions-vault-main/20 - Definitions/DNS\|DNS]] - `cisco-capwap-control` resolves the IP of the WLC
	- Local [[CISCO/ccna-definitions-vault-main/20 - Definitions/IP subnet\|subnet]] broadcast
- *Zero-Touch Configuration* can can also be used with [[CISCO/ccna-definitions-vault-main/20 - Definitions/Cisco DNA Center\|Cisco DNA Center]] to configure other network devices
- *ZTP* is also a cloud-based service hosted by Cisco that allows [[vBond Orchestrator\|vBond Orchestrator]]s and [[vEdge Router\|vEdge Router]]s to connect to each other

# Metadata
### OSI or TCP/IP Layer

### CCNA Exam Topic

### Contributors

### Sources
