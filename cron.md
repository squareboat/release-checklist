1. Crons follow rule of silence (When a program has nothing surprising, interesting or useful to say, it should say nothing Don't produce any stdout when your cron'ed application completes successfully.)
1. Don't pipe any output to /dev/null.
1. Do produce meaningful stderr output when something goes wrong.
1. Do set a $MAILTO address in the crontab to send that error output to the required team.
1. Do call "logger" along with writing to stderr when something goes wrong.