Step3, Method 1: online installation
1) Log onto the Raspberry Pi users system to command line (The initial user name: pi Password: raspberry) 
2) Execute the following command in SSH: 
 git clone https://github.com/goodtft/LCD-show.gitchmod -R 755 LCD-show cd LCD-show/ sudo ./LCD35-show 
3)Wait a few minutes,the system will restart automaticall , enjoy with your LCD


How to Calibrate the Touch Screen 

Install Xinput
cd /boot

cd LCD-show

sudo dpkg -i -B xinput-calibrator_0.7.5-1_armhf.deb

 
2、Execute touch calibration commands: 

DISPLAY=:0.0 xinput_calibratorudas ver video 

  https://www.youtube.com/watch?v=n1COKzM1FlI 
  
  
  Cuando la posicion del cursor esta rotada.
  
  sudo nano ~/.kivy/config.ini
  [input]
mouse = mouse
hid_%(name)s = probesysfs, provider=hidinput,param=invert_y=0

