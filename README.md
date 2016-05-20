# ubuntu /etc/init.d/ script for [open-falcon](http://open-falcon.org/)

copy these files to /etc/init.d/
```
    sudo cp falcon-* /etc/init.d/ && sudo chmod +x /etc/init.d/falcon-*
```

startup when system boots
```
    cd /etc/init.d/; \
    for x in `ls falcon-*`;do \
        update-rc.d $x defaults; \
    done
```
