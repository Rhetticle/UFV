# Controller
<p align="center">
  <img src="https://github.com/TheZ0/UFV/assets/142558812/0ffbf443-e229-4d18-aff3-8888d7fb01e9"/>
</p>
<p align="center">
  <img src="https://github.com/TheZ0/UFV/assets/142558812/0d266653-376d-4685-8693-76237600f095"/>
</p>

The controller was used to control the UFV's forward/backward movement as well as the nozzle yaw and pitch and the pump. The controller PCB uses and STM32Gxx microcontroller to monitor joystick positions and transmits this out via I2C
through a standard USB cable where D-/D+ lines are used for SDA and SCL. On power up, the controller sends a random string of characters to the receiving board mounted on the UFV and waits for them to be echoed back as a form of
communication integrity/error checking. 
