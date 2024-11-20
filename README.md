In this project a basic sensor fusion is realized to enable basic orienation monitoring of the EP3751-0260.
Reporting Issues and feedback is very welcomed.

You find a PLC HMI for monitoring the rotation/orientation of the box:
![image](https://github.com/user-attachments/assets/7c7ef763-f15c-4826-8145-d30de78c70d2)
You can set a zero position a see the rotation via a rotary axis.
The X/Y/Z-axes (3 gauges on the top) will give you the acceleration data.
The euler angles (3 gauges on the bottom) will be stable, even if you make complex movements, like simultaniously rotate via multiple axes.

Application hints (tested configuration & best practice):
- PLC cycletime 250us => full 4kSps of Sensor
- Enable DC operation of box:![image](https://github.com/user-attachments/assets/b24720d0-aecc-44f6-9d42-feff7825d100)

For questions/feedback: A.Kulla@beckhoff.com
