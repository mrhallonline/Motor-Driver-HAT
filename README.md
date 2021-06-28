# Motor Driver HAT For Raspberry Pi

Motor Driver HAT for Raspberry Pi is a module designed to control 2 DC motors simultaneously with I2C communication. It has a powerful onboard chip PCA9685 which provides 12-bit hardware PWM to adjust the motor speed. The logic voltage is 3.3 V with the motor driver TB6612FNG. It can be powered from a battery through the VIN terminal which makes a better experience for the user.

## How To ?

* Stack Motor driver HAT on Raspberry Pi 40 Pin header.

* Connect peripherals with Motor driver HAT as shown in below circuit diagram and turn on slider switch to turn on the Raspberry Pi.

<img src="https://learn.sb-components.co.uk/images/b/b3/Motor_driver_hat_ckt.png" />

* Now open the terminal and run the below command to clone the Github repository of Motor driver HAT.

``` git clone https://github.com/sbcshop/Motor-Driver-HAT.git ```

* Now enter the downloaded folder by running the below command.

``` cd Motor-Driver-HAT ```

* Now run the "Demo.py" python file by running the below command to move motors.

``` python3 Demo.py  ```
