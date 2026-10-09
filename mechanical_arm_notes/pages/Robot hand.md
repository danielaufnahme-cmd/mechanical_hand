tags:: project
status:: buying parts
started:: [[Oct 8th, 2026]]

- ## Plan
	- 3D-printed hand, just the fingers and palm. One servo per finger pulls a string to close it, and a rubber band opens it again.
	- **PC → USB-C → ESP32-S3 → 5 servos.** The servos run on the 5 V adapter; only GND is shared with the ESP32.
	- [Wiring plan](file:///home/daniel/Projects/robot-hand/hand-wiring.html) · [3D animation](file:///home/daniel/Projects/robot-hand/hand-3d.html)
- ## Bought, **€98.32** for the hand
	- **ESP32-S3 board**: the brain, taken from the Freenove kit (€34.95) but counted as €10.99. [Amazon](https://www.amazon.es/dp/B0BMQB2MG1)
	- **Miuzei 15 kg servo ×5**: one per finger, €30.99. [Amazon](https://www.amazon.es/dp/B0BTYRBBFY)
	- **Tesfish 5 V 10 A adapter**: powers the servos, €24.99. [Amazon](https://www.amazon.es/dp/B083QNN7Z7)
	- **DC jack 5.5 × 2.5 mm**: the adapter plugs in here, red to +5 V and black to GND, €3.69. [AliExpress](https://es.aliexpress.com/item/1005012652732602.html)
	- **Capacitor 2200 µF 16 V ×10**: one goes across the servo power with the stripe to GND, €2.56. [AliExpress](https://es.aliexpress.com/item/32812576995.html)
	- **ELEGOO PLA+ 2 kg, grey**: filament for the hand, print at 205–220 °C with the bed at 60 °C, €23.14.
	- AliExpress shipping was €1.96. Paid in total with the whole kit: €122.28.
- ## Already have
	- String, rubber bands, the Ender 3 V3 KE, female jumper wires and Wago connectors (need 4 × 5-hole).
- ## Before ordering
	- Remove the YIXISI 5.5 × 2.1 DC kit from the Amazon basket, it's the wrong size.
	- Have a USB-C data cable for the board.
	- Hinge pins can be bits of 1.75 mm filament or M2/M3 screws.
- ## Maybe
	- TPU 95A filament for grippy fingertips.
- ## Later
	- 6-axis arm with DS3218 20 kg servos and a PCA9685 driver.
	- Webcam hand tracking to move the fingers.
	- Sync these notes with Syncthing.
- ## Decisions
	- 15 kg servos, because 9 g micros (about 2 kg·cm) are too weak for a 9.5 cm finger.
	- 180° or 270° servos are fine, never 360°.
	- USB only powers the ESP32 (0.9 A max, the servos can pull 10 A).
	- 16 V 2200 µF capacitor: 6.3 V is too close to 5 V and 220 µF is too small.
	- No screen for now.
	- Pins, still to check against the Freenove pinout: **Thumb 1 · Index 2 · Middle 14 · Ring 21 · Pinky 47**
