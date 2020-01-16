# dde-calendar
Calendar for debian Desktop Environment.

# debian

* doesn't work without dde-api under debian ..., you must manual install it first.
    * depends

            blur-effect
            rfkill
        
* install depends(If you want to compile it.)
        
        apt install cmake make gcc deepin-gettext-tools libdtkwidget-dev qtbase5-dev-tools \
        qt5-default qtbase5-dev-tools qt5-qmake qtbase5-dev qttools5-dev-tools g++

* compile
        
        cd /path/dde-calendar
        cmake /path/dde-calendar
        make 
        sudo make install

* remove
    
        sudo rm -rf /usr/local/share/dde-calendar
        sudo rm /usr/local/share/applications/dde-calendar.desktop
        sudo rm /usr/local/share/dbus-1/services/com.deepin.Calendar.service
        sudo rm /usr/local/share/icons/hicolor/scalable/apps/dde-calendar.svg
        sudo rm /usr/local/bin/dde-calendar
