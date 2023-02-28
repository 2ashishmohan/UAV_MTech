# Intalling QGroundControl 

## Install QGroundControl for Ubuntu Linux 16.04 LTS or later:

Add current user accout to dialout group and remove modemmanager
```
sudo usermod -a -G dialout $USER
sudo apt-get remove modemmanager
```

Download QGroundControl.AppImage 
```
wget https://s3-us-west-2.amazonaws.com/qgroundcontrol/latest/QGroundControl.AppImage
```
Change permissions and run 
```
chmod +x ./QGroundControl.AppImage 
./QGroundControl.AppImage  (or double click)
```

## Run SITL and connect with Q Ground

```
cd ~/ardupilot/ArduCopter/
sim_vehicle.py
```

