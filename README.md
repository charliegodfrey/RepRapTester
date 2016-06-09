# RepRapTester - An Arduino Open Source 3D printable tensile tester
An Open Source 3D printed tensile strength tester using Arduino for about £30

Things needed:
  1. Arduino Nano/Uno
  2. HX711 load cell amplifier
  3. 300mm section of 51mm square aluminium tubin
  4. 1 Stepstick/DRV8825 stepper driver
  5. 10kg bar load cell
  6. Some 3D printed parts
  7. Nema 17 stepper motor
  8. Flexible coupling (5mm at one end and 8mm at the other)
  9. A section of M8 studding
  10. A micro-switch
  11. A push-to-make button switch


 This Arduino electronics and code performs the following stages:
  
  1. Drives the stepper motor back to the limit switch
  2. Drives the stepper motor to allow placement of the specimen
  3. Zeros the load cell
  4. Waits for pressing of Start button before starting the test
  5. Drives the stepper motor at a set rate (specified in the sketch) whilst printing stress and strain data to the serial terminal
  6. Stops after travelling 30mm (Assumes the specimen has already broken after this movement)
