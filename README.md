# cheese-swiss-snippets
Just a bunch of code snippets to identify and remediate common Active Directory Certificate Services issues.

## Check current configuration
````
certutil -getreg CA\AuditFilter
````

## Enable all auditing
````
certutil –setreg CA\AuditFilter 127
net stop certsvc
````
