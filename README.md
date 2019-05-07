# AsyncHttps #

Uses Runspaces to issue async http requests.

***WARNING!*** This module is configured to:

1. Ignore invalid certificates
2. Ignore insecure protocols

## Outputs ##

System.Object[]

    Uri         - Request Uri
    Status      - Http Status Code or Exception Message
    BeginTime   - Job Start Time
    EndTime     - Job End Time

## Example ##

```powershell
Import-Module AsyncHttps
Invoke-AsyncHttps -DnsName www.contoso.com -UriPaths $('dir1','dir2','dir3')
```

## Reference ##

[https://devblogs.microsoft.com/scripting/beginning-use-of-powershell-runspaces-part-1/](https://devblogs.microsoft.com/scripting/beginning-use-of-powershell-runspaces-part-1/)
