# NAME

**dotf**


# DESCRIPTION

Manage, backup, develop, sync your .dotfiles with ease


# USAGE

```bash
dotf [-AapufhV] [-a|a|--add|add <files>] [-A|A|--all|all|add-all]
     [-u|u|--up|up|--upload|upload [message]] [--fzf|fzf]
     [-h|h] [--help|help] [-V|--version] [-- <git command|git options>]]
```

```bash
dotf [-AapufhV]
```

```bash
dotf [options] [-- <git command|git options>]
```

```bash
dotf [git subcommand]
```


# OPTIONS

```
-a, --add, a, add <files>
```

Add files to be tracked *(git add)*

```
-A, A, --all, add-all
```

Add all tracked files that have been modified

```
-u, u, --up, --upload [message]
```

Commit and push changes, including an option commit message

```
-- <git commands|git options>
```

Run git commands


# META OPTIONS

```
-h, h
```

Show the help menu

```
--help, help
```

Show the full **dotf** help menu

```
--usage, usage
```

Show **dotf** usage

```
--examples, examples
```

Show **dotf** examples

```
-V, --version
```

Show **dotf** version


# EXAMPLES

Running '**dotf**' with no subcommands, options, or arguments
will show the current status of the repository: *(Equivalent to running: '**dotf** status')*

```bash
$  dotf
```

Adding all modified files currently checked into **dotf**.
It will not add new files that are not being tracked.

```bash
$  dotf add-all
```


These next two command will do the exact same thing.
Showing you how the subcommands/options can be used.

These examples will commit and push changes to the remote repository
with a commit message of '*Added help menu to function*'

```bash
$  dotf upload 'Added help menu to function'
```

```bash
$  dotf --upload='Added help menutofunctinon'
```


This little command is a shorthand way of running multiple commands
to add all modified files that are checked into **dotf**, commit changes
with a commit message of '*Expanded help menu*', and then pushing to the remote.

```bash
$  dotf a && dotf 'Expanded help menu'
```


# MORE

For more information, view the README on the [dotf repository](https://github.com/connerwill/dotf)

* *https://github.com/connerwill/dotf*
