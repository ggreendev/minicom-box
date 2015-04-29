# minicom-box

This Docker file builds an Alpine linux based container with minicom.
The default for it's run is baudrate=115200 , device=/dev/mydevice
Enviroment variables: $device , $baud

When starting it runs:
minicom -D $device -b $baud: use can change them using the '-e' at run command

Default run: run -it -e  "baud=new_number" "device=newdevice" --device=/dev/hostdevice:/dev/mydevice



