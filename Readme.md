[![Githbu actions build status](https://img.shields.io/github/workflow/status/jappeace/persistent-event-source/Test)](https://github.com/jappeace/persist-event-source/actions)
[![Hackage version](https://img.shields.io/hackage/v/template.svg?label=Hackage)](https://hackage.haskell.org/package/persistent-event-source) 

Persistent based event sourcing.

TODO:

+ [ ] Add event ordering code.
+ [ ] Prove correctness of event ordering.

I'd like to also add the reapply in a transaction
code, we'd need to refactor so the tables are known
by the system so we can automatically generate a truncate query.

## Usage

### Modifying for your project
Assuming the name of your new project is `new-project`.

```
git clone git@github.com:jappeace/persistent-event-source.git new-project
cd new-project
```

### Tools
Enter the nix shell.
```
nix-shell
```
You can checkout the makefile to see what's available:
```
cat makefile
```

### Running
```
make run
```

### Fast filewatch which runs tests
```
make ghcid
```
