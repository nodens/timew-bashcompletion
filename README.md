# timew-bashcompletion

Bash completion for [TimeWarrior](https://www.timewarrior.net)

## Installation

1. Clone the repository.
1. Copy or link the bash script to the appropriate place.

### Clone the repository

```
$ git clone https://github.com/lauft/timew-bashcompletion.git
```

### Copy/link the Bash script

You can either copy or symbolic link the bash script to install it.
For global installation the target directory is `/etc/bash_completion.d`:

```
$ cd /etc/bash_completion.d
$ ln -s /path/to/timew_bashcompletion_repo/timew
```

Alternatively you can source the completion script in your current shell.

## Usage

Type a (partial) TimeWarrior command and hit `[TAB][TAB]`

List available commands:
```
$> timew[TAB][TAB]
cancel       diagnostics  help         report       stop         untag
config       export       join         shorten      summary      week
continue     extensions   lengthen     show         tag
day          gaps         month        split        tags
delete       get          move         start        track
```

Complete a partial command:
```
$> timew st[TAB][TAB]
start  stop
```

For `timew tag` you can get a list of available tags after entering an id:
```
$> timew tag @2 [TAB][TAB]
TAG1    TAG2    TAG3
```

## Limits

Currently not all commands are fully supported - work in progress!

## License

This work is licensed under the [MIT licence](https://opensource.org/licenses/MIT).
