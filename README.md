# ECE-Module
Linear Voltage Regulator - LM7815 

Basic Functionality and Characteristics
	Shown above is a linear voltage regulator circuit using the LM7815 from TI instruments. 
  This regulator is designed to output a steady voltage supply of 15 volts and a current of 150 milliamps. 
  The input voltage can range from a minimum of 17.7 volts to a maximum of 35 volts. 
  The input current can range from 500 milliamps to 1 amp. 
  The output voltage can swing from 14.4 to15.6 volts and the output current may drop to 75 milliamps if the device overheats. 

Device Operation
	The user has minimal decisions to make when implementing this design. The only added components recommended by the datasheet are C1 and C2. 
  C1 is a bypass capacitor that has the recommended value of 0.22uF. This is used to filter out any unwanted AC voltage. 
  It is stated that this component is not necessary if the device is less than 6 inches from the power supply. 
  The second capacitor has the recommended value of 0.1uF and is used to help clean the signal being output from this device and help the transient response. 
  It is not required for operation but helps in the operation of this device. 

Data Sheet Link: https://www.ti.com/lit/ds/symlink/lm340.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1644099270827&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm340

Digikey Link: https://www.digikey.com/en/products/detail/texas-instruments/LM7815CT/4090887




Adjustable Voltage Regulator - LM117

Basic Functionality and Characteristics
	Shown above is an adjustable voltage regulator circuit using the LM117 device from TI instruments. 
  The regulator is designed to output a steady voltage in the range of 1.25 to 37 volts based on voltage supplied to the input and adjustable pin. 
  This device is designed to output a current of 1.5 amps. The required input voltage is 4.2 to 40 volts. 
  The input voltage also impacts the possible output voltage the device can produce and it is up to the user to degin the circuit to meet their desired requirements. 

Device Operation
	The equation that governs the relationship between the component and input values and the output voltage of the device is listed below:
Vout =1.25v * ( 1 + R2R1)+Iadj * (R2) 
As shown in the equation, the resitance values of R1 and R2  greatly impact the output voltage from the device as well as the current being supplied to the adjustable pin. 
Generally speaking, the greater the value of R2 or the current being supplied to the adjustable pin, the greater the voltage output. 
The other two components in this circuit are capacitors designed to help improve the clarity of the signal being supplied to the device and the output of the device. 
C1 is a bypass filter designed to filter out any unwanted AC voltage from the power supply and is not necessary if the device is less than 6 inches away from the power supply.
C1 has the suggested value of 0.1uF. C2 is used to help clean the output signal and help the transient response of the device. 
This capacitor is completely optional but, is helpful to the operation of the device. This capacitor is recommended to have a value of 1uF.

Data Sheet Link: https://www.ti.com/lit/ds/symlink/lm117.pdf?HQS=dis-dk-null-digikeymode-dsf-pf-null-wwe&ts=1644178138611&ref_url=https%253A%252F%252Fwww.ti.com%252Fgeneral%252Fdocs%252Fsuppproductinfo.tsp%253FdistId%253D10%2526gotoUrl%253Dhttps%253A%252F%252Fwww.ti.com%252Flit%252Fgpn%252Flm117

Digikey Link: 
https://www.digikey.com/en/products/detail/texas-instruments/LM7815CT/4090887

Importing these Schematics 
There are multiple different ways a user could import these designs into their own project. 
A user could either remake these circuits in their own hierarchy sheets in Diptrace or copy and paste the given circuits using the files provided. 
Either way, it is important that, in dip trace, an additional sheet is created in schematic design and, using the properties tab after right-clicking the sheet, 
is changed to be a hierarchy. This allows the user to label the different inputs and outputs with I/O pins. Once all of the pins are labeled and the design is completed. 
A user is able to go to any other sheet and insert the entire circuit repeatedly as a hierarchy. 
This is done by going to the sheet that the user wants to insert the circuit into and using the objects tab at the top of the dip trace. 
The user then selects hierarchy and can choose from the objects they have already designed. 
The object will show up as a simple box with a number of labeled inputs and outputs that are equal to the I/O pins created in the hierarchy circuit. 
This process is done to simplify designs and save time when a circuit is needed repeatedly throughout a single design. 


