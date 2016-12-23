
dmotd is a custom / semi dynamic motd, written to help identify items on a linux box upon login.

 == Instructions ==

cd /usr/local/sbin/

git clone https://github.com/dcnoye/dmotd.git

crontab -e

then add that following:

*/15 * * * * /usr/local/sbin/dmotd > /etc/motd 2>&1
