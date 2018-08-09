# House-of-Helen
home automation project
Raspberry pi, arduinos and D1
Home automation based on Home assistant OS. Includes google assistant (separate unit)
light control, temperature and ventilation, security (will not be displayed here), audio, vacuumrobot, roboHMI,remote communication

RPI1: 3b+, Master controller, Hassbian, wall mounted with touchscreen, frontend: graphic interface
RPI2: 3b, Slave, Google Aiy, only component with internetaccess, controls RoboHMI
Arduino Duemilanova: Slave, sensory inputs
Arduino UNO1: slave, Windowcontroller front, wifi, sound detector, light detector
Arduino UNO2: slave, Windowcontroller back, wifi, sound detector, light detector, rain sensor
Wifi surveillance camera

Available controllers, not assigned yet:
Arduino UNO3
Arduino UNO4
Arduino UNO5
Arduino NANO
Arduino MEGA
D1 mini
Raspberry ZeroW1
Raspberry ZeroW2
Raspberry pi A

So my plan is to have the main RPI control all slaves through wifi. The Google aiy will be my vocal interface to take commands which will be send to the master, also the Google aiy will give me feedback about current status of stuff in the house (i.e. doorbell is pushed > "there is someone at the door")The roboHMI will just be a head with some servo's and light and audio, to give it a more personal feel.
The duemilanova will have inputs from: temperaturesensor, humiditysensor, pirsensor, soundsensor, and controls the gate to the backyard. back and forth communication through Wifi.
Home assistant OS provides a tool for gps controlled actions, so there will be a tracker in my vehicle, and when i move towards my house it will turn on the lights and open the backyard gate.
That same gate will have a rfid/nfc reader, so it can also be opened on demand by presenting my rfid tag.
Same thing for my backdoor, lock is controlled through rfid activation

All audio in the house will be controlled from 1 device. Sources can be: mobile phone, tv, audio player. Speakers are placed in several locations. connectivity: bluetooth, hardwire. So phone calls, playing music, watching tv, alarm, everything uses the same audio system. all speakers can be set individually, per sector.
