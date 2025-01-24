# experimento73
This code is from the FEE230 class (Extensão Unicamp).

The PK2 board will be using during the experiment. The PK2 board is an esp12e (wifi module) + ESP8266 (uC from Espressif), also known as NodeMCU + base board.

## Environment and Level 1 - Physical

On Arduino IDE, go to 'File' -> 'Preferences' and add the link: http://arduino.esp8266.com/stable/package_esp8266com_index.json, then go to 'Tools' -> 'Port' and select the 'COMx' port that the NodeMCU is connect.

![image](https://github.com/user-attachments/assets/979b6436-f380-4627-abb8-22e051936825)

We must upload the following code on the PK2 board: NIVEL_1 -> N1_EXP_7.3_Gerencia-TpM-RSSF.ino. On the green field, inset the name (SSID) of the wireless network that the PK2 will connect. On the Yellow field, insert its password.

![image](https://github.com/user-attachments/assets/ea95f477-3d22-4834-9266-7241d483484d)

On my WiFi Modem, I can see that the sensor is connected.
![image](https://github.com/user-attachments/assets/057de21d-8716-4930-a3a8-4ec4c5b03b9e)

It is important to know in which port the PK2 will be connected: 

![image](https://github.com/user-attachments/assets/d35b4837-f5ef-4840-8e72-bcf442b5a19d)

The IP is also presented on the Arduino's IDE serial monitor:

![image](https://github.com/user-attachments/assets/8c2a3ad6-7f41-43c8-8116-acc4213e8682)

## Level 2 - Connectivity (void)

Radio conection, data being transmitted.

## Environment and Level 3 - Gateway, Base Node

First, download [Python](https://www.python.org/downloads/). In my case, it is version 3.13.1. After the download is complete, run the executable file. Tick the 'Add python.exe to PATH' option. After the installation proccess is complete, open the Command Prompt and run a 'pip install serial'.
Later, to run the  NIVEL_6_EXP_7.3_Gerencia-TpM-RSSF.py, using the command prompt, also install: 'pip install matplotlib',

On NIVEL_3 -> NIVEL_3_EXP_7.3_Gerencia-TpM-RSSF.py, right click and Edit with IDLE 3.13. Then go to Run Module (F5). Then Enter IP and Port.

![image](https://github.com/user-attachments/assets/244e8f48-f889-473b-bbd5-5cf93e21d285)

## Level 4 - Storage

A few txt files. Only written file is the PARAMETROS.txt 

![image](https://github.com/user-attachments/assets/540591bf-7952-41dd-8be0-5731b9104190)

## Level 5 - Abstraction

Go on NIVEL_5 -> NIVEL_5_EXP_7.3_Gerencia-TpM-RSSF.py and open a new IDLE for this python. Run Module.

![image](https://github.com/user-attachments/assets/3390133c-b8f3-4517-9119-0c737353c4d9)

## Level 6 - Front End

Go on NIVEL_6 -> NIVEL_6_EXP_7.3_Gerencia-TpM-RSSF.py and Run Module. On CONFIGURAÇÕES -> Qntd. de Medidas, input a value, such as 1000 (number of packets sent).

![image](https://github.com/user-attachments/assets/46245e49-b609-42ca-ae8e-10e5dda31e02)

Now on Level 4, we have a log file storaged over there:

![image](https://github.com/user-attachments/assets/1151fc94-b948-4161-8e32-d22211b23b0b)

Open those on an excel file, and change them from texto to column, separating them with the ; symbol.

![image](https://github.com/user-attachments/assets/895b54f4-9042-41d7-9a1a-9fa47a866ee5)



