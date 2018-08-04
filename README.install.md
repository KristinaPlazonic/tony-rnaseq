
The app needs to be listed in one of the tabs, so add category: Interactive Apps to manifest.yml
scl enable rh-ruby22 nodejs010 git19 bash
bin/rake assets:clobber
bin/rake assets:precompile
which will create public/assets dir which you have to copy over to /var/www/ood/apps/sys/example-batch/public 
(chown -R root:root /path/to/dir of course)
remove database from /home/kp807/ondemand/data/sys/example-batch/production.sqlite3  (so sys can create a new one)
kill any processes that are running that are Passenger process

