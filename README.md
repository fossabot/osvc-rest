# osvc-rest

An (under development) CLI for using the [Oracle Service Cloud REST API](https://docs.oracle.com/cloud/latest/servicecs_gs/CXSVC/) written in Go.

## Installing Go (for Windows)
[Installation options are available on the Go website](https://golang.org/doc/install#windows).

Make sure that you follow the instructions about adding system variables.

You will want to create a folder exclusively for your Go projects.

[Read more about what you will need to set up to get Go-ing. (I'm sorry for the bad pun)](https://github.com/golang/go/wiki/SettingGOPATH)
   
## Installation

    $ cd ..<go projects folder>
    $ git clone https://github.com/rajangdavis/osvc-rest.git
    $ go build
   
## Compatibility

Go works everywhere; [learn how at this link.](https://dave.cheney.net/2015/08/22/cross-compilation-with-go-1-5)

## Usage
	$ osvc-rest --help
	osvc-rest - a Command Line Interface application to work with the Oracle Service Cloud REST API

	Usage:
	  osvc-rest [command]

	Available Commands:
	  help        Help about any command
	  query       Runs one or more ROQL queries
	  report      Runs an analytics report command

	Flags:
	  -a, --annotate string    Adds a custom header that adds an annotation
	      --demosite           Change the domain from 'custhelp' to 'rightnowdemo'
	  -e, --exclude-null       Adds a custom header to excludes null from results
	  -h, --help               help for osvc-rest
	  -i, --interface string   Oracle Service Cloud Interface to connect with
	      --no-ssl-verify      Turns off SSL verification
	  -p, --password string    Password to use for basic authentication
	  -s, --suppress-rules     Adds a header to suppress business rules
	  -u, --username string    Username to use for basic authentication
	  -t, --utcTime            Adds a custom header to return results using Coordinated Universal Time (UTC) format for time
	  -v, --version string     Changes the CCOM version (default "v1.3")

	Use "osvc-rest [command] --help" for more information about a command.