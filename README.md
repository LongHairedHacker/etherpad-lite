# Etherpad-lite fork of the Fachschaft Informatik at the university Kaiserslautern

This fork only exists to implement small changes required by the Fachschaft Informatik  at the university Kaiserslautern.
If you are looking for etherpad-lite please check the offical repository: https://github.com/ether/etherpad-lite

The software in this repository is not inteded to work anywhere in the world outside our servers !

# Installation

Etherpad works with node v0.8, v0.10 and v0.11, only. (We don't support v0.6)

You'll need gzip, git, curl, libssl develop libraries, python and gcc.  
*For Debian*: `apt-get install gzip git-core curl python libssl-dev pkg-config build-essential`  

Additionally, you'll need [node.js](http://nodejs.org) installed, Ideally the latest stable version, be careful of installing nodejs from apt.

**As any user (we recommend creating a separate user called etherpad):**

1. Move to a folder where you want to install Etherpad. Clone the git repository `git clone git://github.com/longhairedhacker/etherpad-lite.git`
2. Change into the new directory containing the cloned source code `cd etherpad-lite`

Now, run `bin/run.sh` and open <http://127.0.0.1:9001> in your browser. 

Update to the latest version with `git pull origin`. The next start with bin/run.sh will update the dependencies.

You like it? [Next steps](#next-steps).

# Next Steps

## Tweak the settings
You can initially modify the settings in `settings.json`. (If you need to handle multiple settings files, you can pass the path to a settings file to `bin/run.sh` using the `-s|--settings` option. This allows you to run multiple Etherpad instances from the same installation.)  Once you have access to your /admin section settings can be modified through the web browser.

You should use a dedicated database such as "mysql", if you are planning on using etherpad-in a production environment, since the "dirtyDB" database driver is only for testing and/or development purposes.

# License
[Apache License v2](http://www.apache.org/licenses/LICENSE-2.0.html)
