# ZSH Reference

## Aliases
* `mcd	mkdir -p $1 && cd $1`
* `l	ls -lh`
* `ll	ls -lah`
* `la	ls -ah`
* `dir	ls -lhR --color=auto | less`
* `llog	less /var/log/syslog`
* `tlog	less +F /var/log/syslog`

### apt
* `acs	apt-cache search`
* `acsh	apt-cache show`
* `agi	apt-get install`
* `agud	apt-get update`
* `agug	apt-get upgrade`
* `agdug	apt-get dist-upgrade`

### pacman
* `pacupg`: `pacman -Syu` Sync repos and upgrade packages
* `pacin`: `pacman -S` Install package
* `pacre`: `pacman -R` Remove package but keep config and deps
* `pacrem`: `pacman -Rns` Remove package with config and deps
* `pacinfo`: `pacman -Si` Display info about a repo package
* `pacs`: `pacman -Ss` Search the repo for a package
* `pacloc`: `pacman -Qi` Display info about a local package
* `paclocs`: `pacman -Qs` Search local installed package


## Global Aliases
* `L	| less -M`
* `G	| grep -i --color`
* `T	| less +F -M`


## Hotkeys
* `Esc-h`		Show help for first word in cmdline
* `Esc-i`		Trigger completion
* `Esc-e`		Edit commandline in vim
* `Ctrl-i d`	Insert timestamp (YYYY-MM-DD)
* `Ctrl-o s`	Prefix commandline with sudo
* `Ctrl-space`  Expand abbreviations
* In complete-mode:

  * `Ctrl-n`	Take selection and complete again
  * `Esc return`  Take selection as argument, dont close completion


## Functions
* `greph`		History grep
* `new`		List files modified within the last X days
* `H-Glob`	Globbing help
* `H-Abbrevs`	List of defined abbreviations
* `calc`		A tiny calculator


## ZSH-Globbing
* `**/*.pdf	recursive all pdf-files
* `**/*(.)	recursive all files
* `**/*(/)	recursive all directories

### Qualifier
* `(f:gu+w,o-rx)`	Permissions
* `(u:user)`		User match
* `(g:group)`		Group match
* `^`		Negate all following qualifier 


## More ZSH-Tricks
* `zmv '(*).bak' '$1'`	Umbenennen mit regex
* `for i (*.eps) epstopdf $i`

