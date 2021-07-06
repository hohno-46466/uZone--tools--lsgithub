# uZone--tools--lsgithub/README

This is a manual page of the lsgithub command.

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

* GNU getopt
* jq

You must set the full path name of the gnu getopt command to the ggetopt variable in this lsgithub script.
Similarly, you must set the full pathname of the jq command properly in the jq variable.

#### (GNU getopt command)

   If you already have /usr/bin/getopt and it's a GNU getopt, you don't need to prepare GNU plot

   If you don't and you are using macOS, install it by "brew install gnu-getopt"

   If you are using Linux or WSL on Windows, you can insatll it by using apt command or similar package manager on your distribution.


#### (JQ command)

   If you don't have /usr/bin/jq, install it by yourself.

   If you are using macOS and using homebrew, you can install it by "brew install jq"

   If you are using Linux or WSL on Windows, you can install it by using apt command or similar package manager on your distribution.



## PREPARATION

Prepare your access token. Then your github user name and the access token must be written in the "secret file" with the following format:

GITHUB_USER=your_github_name

ACCESS_TOKEN=your_acess_token

The secret file is $HOME/.secret/lsgithub, but you can change it to another file by changing the SECRET_FILE variable in this lsgithub script.
It is highly recommended to change the permissions of the directory where the secret file is located ($HOME/.secret/ by default) to 700, and change the permissions of the secret file ($HOME/.secret/lsgithub by default) to 600.

You can learn how to get the access token here:
https://docs.github.com/en/github/authenticating-to-github/keeping-your-account-and-data-secure/creating-a-personal-access-token

## RETURN VALUE

If lsgithub finds any problems, a non-zero exit code is returned.

## BUGS

Not reported but has some?

## LICENSE

undefined.

## AUTHOR(S)

[hohno-46466](https://github.com/hohno-46466)  (@hohno_at_kuimc)

## SEE ALSO

See 00README.txt, if prepared.

Mon Jun 14 23:29:52 JST 2021
