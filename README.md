[Ongoing project]3DS Power Off

The idea is to create a 3ds software to power off the console without pressing the power button. Or at least trigger the application closed menu with the touch screen option to power off.

Tap to power off.(Broken, still using trail & error to find the apt service used to trigger power off)

Holding L button exit the app and can also be used to return back to the EmuNand after playing a game that uses additional resources form the menu.

Holding R button kicks you out of the Emunand back into SysNand.

Power off function is still broken. Something needs to be fixed. There is an alternate method to power off and it requires writing a value of 8 to one of the I2C registers, (REGISTER:0x20, WIDTH:8) on device 3. But this method is potentially dangerous? 

Credits:
Smea for creating ctrulib which build the base foundation for making homebrews etc.
Code is based off AlbertoSONIC's Quick Reboot. I modified the HID inputs and added power off code.
