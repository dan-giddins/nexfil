**NExfil** is an **OSINT** tool written in python for finding profiles by username. The provided usernames are checked on over 350 websites within few seconds. The goal behind this tool was to get results quickly while maintaining low amounts of false positives.


## Features

* **Fast**, lookup can complete **under 20 seconds**
* Over **300** platforms are included
* Batch processing
  * Usernames can be provided from command-line
  * List of usernames can be provided from a file
* Results are automatically saved in txt file

## Usage

```bash
$ nexfil --help
usage: nexfil [-h] [-u U] [-f F] [-l L] [-t T] [-v] [-U] [-pm PM] [-proto PROTO] [-ph PH] [-pp PP]

nexfil - Find social media profiles on the web | v1.0.5

options:
  -h, --help    show this help message and exit
  -u U          Specify username
  -f F          Specify a file containing username list
  -l L          Specify multiple comma separated usernames
  -t T          Specify timeout [Default : 10]
  -v            Prints version
  -U            Check for Updates
  -pm PM        Proxy mode [Available : single, file] [Default : single]
  -proto PROTO  Proxy protocol [Available : http, https] [Default : http]
  -ph PH        Proxy Hostname
  -pp PP        Proxy port -U          Check for Updates
```

> Single username

```bash
nexfil -u useranme
```

> Multiple *comma* separated usernames

```bash
nexfil -l "user1,user2"
```

> Username list in a file

```bash
nexfil -f users.txt
```
