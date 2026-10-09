# Mechanical Hand

A 3D-printed, servo-driven robotic hand built around an ESP32-S3.

The project covers only the fingers and the palm. There is no wrist, forearm or elbow; it is just the hand itself.

## How it works

- Five servos, one per finger (thumb, index, middle, ring, pinky).

- Each servo pulls a tendon to close its finger. A rubber band pulls the finger back open when the servo releases.

- An ESP32-S3 drives all five servos and is controlled from a PC over USB.

- The servos run from their own 5 V supply. The PC's USB port only powers the ESP32, because USB cannot supply enough current for five servos.

## Shopping list

| Part | What it's for | Shop | Price |
| - | - | - | - |
| [ESP32-S3 board](https://www.amazon.es/dp/B0BMQB2MG1) | Controls the servos  | Amazon.es | €10.99 |
| [Miuzei 15 kg servo, 180°, ×5](https://www.amazon.es/dp/B0BTYRBBFY) | One per finger | Amazon.es | €30.99 |
| [Tesfish 5 V 10 A adapter](https://www.amazon.es/dp/B083QNN7Z7) | Powers the servos | Amazon.es | €24.99 |
| [DC jack 5.5 × 2.5 mm](https://es.aliexpress.com/item/1005012652732602.html) | The adapter plugs in here | AliExpress | €3.69 |
| [Capacitor 2200 µF 16 V, ×10](https://es.aliexpress.com/item/32812576995.html) | Smooths the servo power | AliExpress | €2.56 |
| ELEGOO PLA+ filament, 2 kg, grey | Printing the hand | Amazon.es | €23.14 |
| AliExpress shipping |  | AliExpress | €1.96 |
| **Total** |  |  | **€98.32** |


Also used, already at hand: string, rubber bands, female jumper wires, Wago lever connectors and a 3D printer (Creality Ender 3 V3 KE).

## Files

- `file\_3d.FCStd`: FreeCAD model of the hand

- `mechanical\_arm\_notes/`: build notes

## Status

Work in progress.

