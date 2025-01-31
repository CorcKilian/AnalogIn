# AnalogIn

The project included here is the basic operation of the analog-to-digital converter (ADC) on the STM32L432KC.
Helper functions have been provided that handle the configuration of the pin modes (`pinMode()`), initialisation fo the ADC (`initADC()`), and reading of the ADC (`readADC()`).
Please ensure you reveiw these function before uplaoding the code to your board.

# Studio task/activity #1

Basic ADC functioning.

- [X] Copy or clone this [repository](https://github.com/paulTUDublin/AnalogIn) and open as a platformIO project.
- [ ] Verify the board is working as you alter the voltage at the input pin using the potentiometer on the board.
- [ ] Configure PA1 as an analog input and read from the appropriate ADC channel and verify the operation by turning on and off the external LED connected to PA3. This [image](https://brightspace.tudublin.ie/d2l/le/content/384173/viewContent/3327044/View) will help.
- [ ] Use a volt meter or oscilloscope to view the input voltage and determine what voltage is required to turn on the LED. *HINT*: what resolution is the ADC?
- [ ] Document any progress/changes in the README.md file (use [Markdown](https://www.markdownguide.org/cheat-sheet/) to format this document.) and upload your project to your GitHub repo. 

