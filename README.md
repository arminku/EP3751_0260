In this project a basic sensor fusion is realized to enable orienation monitoring of the EP3751-0260.
Reporting Issues and feedback is very welcomed.

You find a PLC HMI for monitoring the rotation/orientation of the box:
<img width="855" height="569" alt="image" src="https://github.com/user-attachments/assets/0e2d6fa6-69cd-4020-acf6-76e9bd9f2afd" />

You can calibrate the offset and zero the angles (tara) to monitor the rotation via an axis.
There are different fitler algorithms implemented which are optional to use, but might help for monitoring specific applications.
By using some of the filter algorithms the euler angles (3 gauges Phi (rotation X-axis), Theta (Y) and Psi(Z)) can be stable, even if you make complex movements, like simultaniously rotate via multiple axes.

Application hints (tested configuration & best practice):
- Align PLC cycle and sensor sample rate (F800:0D or set to "Auto" to automatically align):
  <img width="430" height="27" alt="image" src="https://github.com/user-attachments/assets/ee3a09de-c038-495f-bd05-f339c717d7ee" />
- Enable DC operation of box:
  ![image](https://github.com/user-attachments/assets/b24720d0-aecc-44f6-9d42-feff7825d100)
- Use advanced filter created in filter designer and deploy them to module to reduce noise 


