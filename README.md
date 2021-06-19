# uZone--tools--lsgithub/README

====

## NAME

lsgithub - list GitHub repositories

## SYNOPSIS

lsgithub [ options ]

## DESCRIPTION

lsgithub is a utility for displaying information about your GitHub repositories.
lsgithub is written in shellscript.

## OPTIONS

	-l
		long format
	
	-c
		sort by creation time
	
	-t
		sort by last update time
	
	-r
		sort in reverse order
	
	--public
		search public repositories only
	
	--private
		search private repositories only
	
	--all | --everybody
		search both public and private repositories
	
	--owner
		owner mode
	
	--others
		none owner mode

## REQUIREMENT

The following commands must be installed.

* gnu getopt
* jq

## RETURN VALUE

 If lsgithub finds any problems, a non-zero exit code is returned.
 
## BUGS

Not reported but has some?

## LICENSE

undefined.

## AUTHOR(S)

[hohno-46466](https://github.com/hohno-46466)

## SEE ALSO

See 00README.txt if prepared.

Mon Jun 14 23:29:52 JST 2021

