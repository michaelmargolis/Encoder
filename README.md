# Encoder Library

Encoder counts pulses from quadrature encoded signals, which are commonly available from rotary knobs, motor or shaft sensors and other position sensors. 

forked from https://github.com/PaulStoffregen/Encoder version 1.4.3

This version includes code that moves the attachInterrupt calls from the constructor to an implicitly called begin method https://github.com/PaulStoffregen/Encoder/pull/13
That change fixes a problem on platforms such as the Pico that may not correctly handle Arduino API calls from static constructors. 
interrupt_pins.h has defines added for all pico 2040 digital pins but note that lower numbered pins are more efficient than higher numbers 
