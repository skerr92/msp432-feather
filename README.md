# msp432-feather

Welcome to the public repository for my MSP432P401R feather board design. There are just a few things that should be considered when working with this design. 

<image src="images/Screen Shot 2020-07-28 at 7.55.07 PM.png">
  
# Update (07-28-2020): Fixed issues with bad footprint for FT232RL chip

There was a connection and foodprint issue with the FT232RL chip which need to be replaced. That is reflected in the current board and schematic files.

In addition to this, 4 JTAG header pins are also added to allow programming from a MSP432P401R development board.

# Update (07-16-2020)

The schematic and board files were fixed related to the floating TEST pin on the FT232RL IC.

# Update (07-11-2020): If you choose to manufacture the current board uploaded read this first (fixed):

The old schematic is working to be updated following an issue with the FT232RL USB to UART chip. This is easy to overcome when assembling the current board, simply bridge pins 25 and 26 on the board. This ensures that pin 25 (TEST) is tied to pin 26 (GND). According to the FT232R datasheet, the chip won't be recognized because the test pin is floating. This will be corrected in the next revision.

# Get started today

You can get started by ordering the board from OshPark --> <a href="https://oshpark.com/shared_projects/jjmrRj4x">MSP432 Boards on OshPark</a>

# 1

The design is open for revision. If you have experience with PCB design and would like to contribue, I encourage you to do so! Simply create a fork of the repository and you're good to go!

If you are new to PCB design and want to play around with the files, you can do that to! Just download autodesk eagle through autodesk fusion and you can get started.

# 2

The BOM and board files are included for convenience if you so chose to build out this board. I am in the midst of testing the current design so I haven't worked out all the flaws that might be associate with this PCB. 

I should be done with the first board by the end of August, and I'll update the board files, schematic, and the lot as necessary.

# final thoughts

This board is the second board I have been working on and adding the the open source community. With hard work, I hope that this board can be successfully submitted the the Open Hardware Association as a means to help others who want to develop with the MSP432, can do so with the additional support of the Adafruit feather wings and other add-on boards.

If you have any questions, you can open up an issue in the <a href="https://github.com/skerr92/msp432-feather/issues">Issues</a> tab of this repository!

Please check the <a href="https://github.com/skerr92/msp432-feather/tree/master/technical%20documentation">Technical Documentation</a> for additional resources for working with the MSP432P4xxx microcontroller.
