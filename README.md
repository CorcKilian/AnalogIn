# AnalogIn

The project included here is the basic operation of the analog-to-digital converter (ADC) on the STM32L432KC.
Helper functions have been provided that handle the configuration of the pin modes (`pinMode()`), initialisation fo the ADC (`initADC()`), and reading of the ADC (`readADC()`).
Please ensure you reveiw these function before uploading the code to your board.

# Studio task/activity #1

Basic ADC functionality.

- [X] Copy or clone the [AnalogIn repository](https://github.com/paulTUDublin/AnalogIn){target="_blank"} and open as a platformIO project.
- [x] Verify the board is working. As you alter the voltage at the input pin using the potentiometer on the board, does the onboard LED on **PB3** turn on?
- [ ] Configure **PA1** as an analog input and read from the appropriate ADC channel and verify the operation by turning on and off the external LED connected to **PA3** using the ADC input value. This [pinout image](https://brightspace.tudublin.ie/d2l/le/content/384173/viewContent/3327044/View){target="_blank"} will help. You will need an additional LED and resistor ($\approx 100-200 \Omega$).

I did this by including the following code in the setup.
    pinMode(GPIOA,1,3);  // analog input
I also needed to change the main loop to read from ADC channel 1 but pinA1 which is " vin = readADC(6)"


- [ ] Use a voltmeter or oscilloscope to view the input voltage and determine what voltage is required to turn on the LED. *HINT*: what resolution is the ADC? Can this be used to convert between digital units and voltage?
- [ ] Document any progress/changes in the README.md file (use [Markdown](https://www.markdownguide.org/cheat-sheet/){target="_blank"} to format this document) and upload your project to your GitHub repo.
