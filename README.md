
dmotd is a custom / semi dynamic motd(message of the day),
written to help identify items on a linux box upon login.

The included version currently is tailored to a centos/redhat system with openVZ containers, but is easily modified to run on any nix based os.


Instructions

cd /usr/local/sbin/

git clone https://github.com/dcnoye/dmotd.git

crontab -e

Then add that following:

*/5 * * * * /usr/local/sbin/dmotd/dmotd > /etc/motd 2>&1
