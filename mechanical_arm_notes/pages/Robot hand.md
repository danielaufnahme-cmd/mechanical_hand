tags:: project
status:: buying parts
started:: [[Oct 8th, 2026]]

- ## Cost overview — total €98.32
	- | Part | Shop | Option | Price |
	  |---|---|---|---|
	  | ESP32-S3 board (from the Freenove kit) | Amazon.es | counted as one plain ESP32-S3 | €10.99 |
	  | Miuzei 15 kg servo 180° ×5 | Amazon.es | 5 piezas | €30.99 |
	  | Tesfish 5 V 10 A power adapter | Amazon.es | 5V 10A | €24.99 |
	  | DC female connector 5.5 × 2.5 mm (with wires) | AliExpress | DC-022B 5.5-2.5 / 1PCS | €3.69 |
	  | Capacitor 2200 µF 16 V ×10 | AliExpress | 16V2200UF 10PCS | €2.56 |
	  | AliExpress shipping (minus €0.03 discount) | AliExpress | — | €1.96 |
	  | ELEGOO PLA+ filament 2 kg, grey | Amazon.es | Grey, 2 kg | €23.14 |
	  | **Total for the hand** | | | **€98.32** |
	- The hand uses the ESP32-S3 board from the Freenove kit; only that board's value (€10.99) counts toward the build.
	- Actually paid, with the whole kit: €122.28 (Amazon €114.07 + AliExpress €8.21)
- ## Plan
	- Tendon-driven 3D-printed hand. One servo per finger pulls a string; a rubber band on the back opens the finger. Servos sit in the forearm.
	- PC → USB-C → ESP32-S3 → 5 servos. The servos get power from a separate 5 V 10 A plug-in adapter; only GND is shared with the ESP32.
	- Plan pages: [wiring plan](file:///home/daniel/Projects/robot-hand/hand-wiring.html) · [3D animation](file:///home/daniel/Projects/robot-hand/hand-3d.html)
- ## Chosen
	- DONE Freenove ESP32-S3 Basic Starter Kit #chosen
	  name:: Freenove ESP32 Kit ESP32-S3 Camera Board Starter Kit Basic
	  link:: https://www.amazon.es/dp/B0BMQB2MG1
	  option:: —
	  price:: €34.95 (paid) · counted in the build as €10.99 (a plain ESP32-S3)
	  shop:: Amazon.es
	  note:: its ESP32-S3 board runs the hand; the breadboard + jumper wires are used too; the rest is for fun
	- DONE Miuzei 15 kg digital servo 180° #chosen
	  name:: Miuzei 15KG Digital Servo Motor Metal Gear High Speed Torque Servo Motor for RC Car 1:8 1/10 12 Helicopter Airplane Car Boat Robot Control Arm 5PCS
	  link:: https://www.amazon.es/dp/B0BTYRBBFY
	  option:: 5 piezas
	  price:: €30.99
	  shop:: Amazon.es
	  note:: 13 kg·cm at 4.8 V, metal gears, 4.5 (936)
	- DONE Tesfish 5 V 10 A 50 W power adapter (EU plug) #chosen
	  name:: Tesfish 5V 10A Power Adapter 50W Transformer Power Supply 5.5 x 2.1/2.5mm for CCTV, Camera, WLAN Router, LED Strip Light WS2811 / WS2812B
	  link:: https://www.amazon.es/dp/B083QNN7Z7
	  option:: 5V 10A
	  price:: €24.99
	  shop:: Amazon.es
	  note:: plug 5.5 × 2.5 mm, centre +; CE, 100–240 V input; 4.2 (126)
	- DONE DC female connector 5.5 × 2.5 mm with red/black wires #chosen
	  name:: 1/2/5 Piezas Conector Hembra de Alimentación DC022D DC022X DC099 DC de 5.5*2.1mm/5.5*2.5mm, Enchufe Impermeable DIY para Montaje en Panel
	  link:: https://es.aliexpress.com/item/1005012652732602.html
	  option:: DC-022B 5.5-2.5 / 1PCS
	  price:: €3.69
	  shop:: AliExpress (Test Board Store)
	  note:: the Tesfish plug goes in; red wire → +5 V Wago, black wire → GND Wago; comes with nut + waterproof cap
	- DONE Electrolytic capacitor 2200 µF 16 V #chosen
	  name:: Condensador electrolítico de alta frecuencia 6,3 V 10V 16V 25V 35V 50V…
	  link:: https://es.aliexpress.com/item/32812576995.html
	  option:: 16V2200UF 10PCS
	  price:: €2.56
	  shop:: AliExpress (ENLINCA PRO Store)
	  note:: one goes across the servo +5 V / GND Wagos; the striped side (−) to GND, the long leg (+) to +5 V; 9 spares
	- DONE ELEGOO PLA+ filament 2 kg, grey #chosen
	  name:: ELEGOO PLA+ Filament 1.75 2kg Grey | PLA Plus for 3D Printer, Dimensional Accuracy +/- 0.03mm, 3D Filament Spool
	  link:: (send me the link)
	  option:: Colour Name: Grey, 2 kg
	  price:: €23.14 (limited-time deal, €11.57/kg)
	  shop:: Amazon.es
	  note:: 2 × 1 kg, 1.75 mm; the hand + forearm use about 300–600 g, the rest is for test prints and the arm. Print at ≈ 205–220 °C, bed 60 °C
- ## To pick
	- LATER TPU 95A small spool, for grippy fingertip pads #optional
- ## Already have
	- String, rubber bands, Creality Ender 3 V3 KE (not enough filament left)
	- Female jumper wires
	- Wago lever connectors (need 4 × 5-hole)
- ## Check before ordering
	- Remove the YIXISI 5.5 × 2.1 DC connector kit (€8.99) from the Amazon basket: wrong size (2.1 mm) and the AliExpress DC-022B replaces it
	- A USB-C data cable from the PC to the board (most phone cables work)
	- Hinge pins for the finger joints: pieces of 1.75 mm filament work (free), or M2/M3 screws
- ## Later
	- 6-axis arm (stronger servos, e.g. DS3218 20 kg; a PCA9685 16-servo driver)
	- Webcam hand tracking → finger angles
	- Sync notes with Syncthing
- ## Decisions
	- The hand uses the ESP32-S3 board from the Freenove kit; for the build cost only the board counts (€10.99).
	- No screen for now (dropped the OLED).
	- Servos must be the 15 kg class. 9 g micros (Miuzei MF90, Behogan) are about 2 kg·cm, too weak for a 9.5 cm finger.
	- 180° or 270° servos are both fine; never 360° / continuous.
	- The PC's USB can't power the servos (0.9 A max vs up to 10 A); it only powers the ESP32.
	- Capacitor: 16 V, 2200 µF. 6.3 V is too close to 5 V; 220 µF is too small; 4700 µF+ is unnecessarily big.
	- Suggested pins (check them against the Freenove pinout sheet; they avoid the camera and SD-card pins): Thumb GPIO 1 · Index GPIO 2 · Middle GPIO 14 · Ring GPIO 21 · Pinky GPIO 47
