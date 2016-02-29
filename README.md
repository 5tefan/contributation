# contirbution + mutation = contributation

Write messages on your profile using the contribution frequency visualization.

Usage: Execute `./script.sh "<message>"` in a Github repo

## How it works

The core of the script wraps calls to `git commit` with the environment variable `GIT_COMMITTER_DATE` and arguemnts set approriately.  

Additionally, commits are made using the commit message "heyy", making them easy to remove. All pervious commits containing "heyy" are removed when the script runs to allow you to edit and change messages. The script is (hopefully) appropriately self contained enough to be run on a cron job that could update you mesage weekly, or as needed to keep it current or properly on the visualization area.

NOTE: Github does not count commits to forked repositories on your visualization so you must run this in your own repository. See [Why are my contributions not showing up on my profile?](https://help.github.com/articles/why-are-my-contributions-not-showing-up-on-my-profile/)
