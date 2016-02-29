# contirbution + mutation = contributation

Write messages on your profile using the contribution frequency visualization.

Usage:
	1. Fork
	2. Execute `./script.sh "<message>"`

## How it works

The core of the script wraps calls to `git commit` with the environment variable `GIT_COMMITTER_DATE` set appropriately to form the message. 

Additionally, commits are made using the commit message "heyy", making them easy to remove. All pervious commits containing "heyy" are removed when the script runs to allow you to edit and change messages. The script is (hopefully) appropriately self contained enough to be run on a cron job that could update you mesage weekly, or as needed to keep it current or properly on the visualization area.


