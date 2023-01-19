```
Help get-item -xxx 
```
can replace ```-xxx``` with -Online or with -Full

PowerShell enables you to do what you already have permission to do.

We use ```set-location``` in PS, but ```cd``` is the equivalent in Bash

```new-item``` followed by ```-itemtype xxx``` can create directories or items in a folder

We can pipe commands using ```|```. An example is get-process | export-csv procs.csv

compare-object takes two sets of info and compares them

When we have issues with multiple modules having the same name for commands we use: ```xx\command```

# Day 6
1. Labq12.txt =>, labq11.txt <=
2. Issue with out-file: cannot process argument because value of argument "path" is null. Out-file won't do anything because the file is created by Export-csv.
3. stop-job can also go by instanceID, state, or filter. You can stop a job without get-job
4. -delimiter "|"
5. -includeTypeInformation
6. -noclobber, -confirm
7. -useCulture

# Day 5
1. new-item Labs -itemtype Directory
2. new-item .\Labs\Test.txt
3. ```set-item .\Labs\Test.txt -value Testing``` does not work because its provider does not support this type of operation
4. get-item env:Path
5. The Filter specifies to qualify the Path parameter, the Include specifies an array of 1+ string patterns to be matched as the cmdlet gets child items and matching items are included, and the Exclude also specifies an array of 1+ but excludes matches from output. All allow wildcards. Include and Exclude must be used with -Recurse or if you are querying a container.

# Day 4
1. gps
2. test-connection google.com
3. get-command -type cmdlet
4. get-alias
5. new-alias "ntst" netstat
6. gps -name p*
7. new-item -path .\MyFolder1 -ItemType Directory
8. remove-item .\MyFolder*

# Day 3
2. Yes, ConvertTo-Html.
3. Yes, redirect.
4. A lot
5. Set-PSBreakpoint
6. xxx-Alias cmdlets are available
7. Start-Transcript and Stop-Transcript
8. get-process
9. -IncludeUserName
10. Invoke-Command
11. 80 characters is the default, you can change the $PSDefaultParameterValues parameter to change the default
12. -NoClobber
13. Get-Alias
14. get-help process
15. 10
16. get-help array