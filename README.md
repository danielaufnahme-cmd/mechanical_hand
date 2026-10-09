# Mechanical Hand

A 3D-printed, servo-driven robotic hand built around an ESP32-S3.

The project covers only the fingers and the palm. There is no wrist, forearm or
elbow; it is just the hand itself.

## How it works

- Five servos, one per finger (thumb, index, middle, ring, pinky).
- Each servo pulls a tendon to close its finger. A rubber band pulls the
  finger back open when the servo releases.
- An ESP32-S3 drives all five servos and is controlled from a PC over USB.
- The servos run from their own 5 V supply. The PC's USB port only powers the
  ESP32, because USB cannot supply enough current for five servos.

## Hardware

- ESP32-S3 board
- 5x 15 kg 180° servos
- 5 V 10 A power adapter

## Shopping list

The full list of parts I bought, with prices, is coming soon.

## Files

- `file_3d.FCStd`: FreeCAD model of the hand
- `mechanical_arm_notes/`: build notes

## Status

Work in progress.
