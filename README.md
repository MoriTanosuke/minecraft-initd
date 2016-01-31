# minecraft-initd
Simple init script used on my Amazon AWS instances running minecraft servers

## How to use this script

Download the script into directory `/etc/init.d` and make it executable

  pushd /etc/init.d && wget https://raw.githubusercontent.com/MoriTanosuke/minecraft-initd/master/minecraft && chmod +x minecraft && popd

Make sure the variable `SERVICE` matches your minecraft server JAR filename. Also check `USERNAME` and `MCPATH`.

Enable the script on system startup on Ubuntu:

  update-rc.d minecraft defaults
