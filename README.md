# kubeclone

kubeclone is a command line tool that helps to clone kubernetes objects between contexts,namespaces and clusters.

## Developement

Clone the repository into your $GOPATH and then build it.

```
$ mkdir -p $GOPATH/src/github.com/chipher-co/
$ cd $GOPATH/src/github.com/chipher-co/
$ git clone https://github.com/cipher-co/kubeclone.git
$ cd kubeclone
$ dep ensure
```

Build

```
$ go build -o kubeclone main.go
```

Run
```
$ go run main.go --help

Kubeclone : 

command line to built to clone kubernetes objects between contexts,namespaces 
and clusters.

Usage:
  kubeclone [command]

Available Commands:
  init        initialises kubeclone
  replicate   replicates kubernetes obejects

Flags:
      --config string   config file (default is $HOME/.kubeclone.yaml)
  -h, --help            help for kubeclone
  -t, --toggle          Help message for toggle

Use "kubeclone [command] --help" for more information about a command.
```