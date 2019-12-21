# Go_CommandLine
### Go command line tool 
### Linux_Academy Course

### Task: 
You've been asked to create a tool to export a system's user information.
The command will be able to export usernames, IDs, home directories,
and shells as either JSON or CSV.
This command will not include information about system users
(users with IDs under 1000). By default, the command will display
the information as JSON to stdout, but the -format flag will allow a
person to specify csv as the export type. Additionally, a file can be
specified by using the -path flag.
Here are the various ways the tools can be used:



```bash
$ hr -format=csv -path=path/to/users.csv
```
```bash
$ hr -path=path/to/users.json
```

```bash
$ hr

[
  {
    "name": "cloud_user",
    "id": 1002,
    "home": "/home/cloud_user",
    "shell": "/bin/bash"
  },
  {
    "name": "kevin",
    "id": 1003,
    "home": "/home/kevin",
    "shell": "/bin/zsh"
  },
]
```
```bash
$ hr -format=csv

name,id,home,shell
cloud_user,1002,/home/cloud_user,/bin/bash
kevin,1003,/home/kevin,/bin/zsh
```
