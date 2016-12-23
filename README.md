

add that following to your crontab:

{{{
*/15 * * * * /usr/local/sbin/dmotd > /etc/motd 2>&1
}}}
