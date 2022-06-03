# bigip-irule-samples
Some usefull iRule samples. The samples are provided as is, and should be used with caution :).

# irule_cve-2022-26134
To lower risk for exploitation of Confluence 0day CVE-2022-26134, Atlassian advice customers to block URIs containing ${. This iRule will do this on a f5 BIG-IP LTM.

Atlassian advisory:
https://confluence.atlassian.com/doc/confluence-security-advisory-2022-06-02-1130377146.html
