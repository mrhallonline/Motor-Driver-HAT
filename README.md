# Motor Driver HAT For Raspberry Pi

Motor Driver HAT for Raspberry Pi is a module designed to control 2 DC motors simultaneously with I2C communication. It has a powerful onboard chip PCA9685 which provides 12-bit hardware PWM to adjust the motor speed. The logic voltage is 3.3 V with the motor driver TB6612FNG. It can be powered from a battery through the VIN terminal which makes a better experience for the user.



## Configure the I2C (''' default is 0x40 ''') 
 * 0x40 is the default address of the motor driver at A5,you can also Change the I2C address which is vary from  0x40 to 0x5F (A0-A5)
 * Default A5 is connected to ground (0v) and rest of A0-A4 are not connected to neither 5v nor ground (means open circuit)
  <img src="https://github.com/sbcshop/Motor-Driver-HAT/blob/main/I2C_configure.JPG" /> 
  
 * You can change resistors of A0-A4 to configure the slave address. If you solder a resistor or short it,The address of the I2C range from 0x40 to 0x5F.
 * For Example :
   * A5 is default 0, and  A0-A4 are disconnected as you see in hardware, it means 0. The I2C slave address is 0x40 (default address)
  <img src = "https://github.com/sbcshop/Motor-Driver-HAT/blob/main/img.JPG" />
  
## How To ?

* Stack Motor driver HAT on Raspberry Pi 40 Pin header.

* Connect peripherals with Motor driver HAT as shown in below circuit diagram and turn on slider switch to turn on the Raspberry Pi.

<img src="https://learn.sb-components.co.uk/images/b/b3/Motor_driver_hat_ckt.png" />

* Change the addrerss by changing the A0-A4



* Now open the terminal and run the below command to clone the Github repository of Motor driver HAT.

``` git clone https://github.com/sbcshop/Motor-Driver-HAT.git ```

* Now enter the downloaded folder by running the below command.

``` cd Motor-Driver-HAT ```

* Now run the "Demo.py" python file by running the below command to move motors.

``` python3 Demo.py  ```
