# YASH build notes

## ERRATA

In the first run of the PCB, the pins for the clock frequency Molex header are mislabeled. The label should say "Clock W/CW", not "Clock W/CCW".

Also in the first run, the LED footprint silkscreen is on the wrong side of the PCB. The LED should of course be mounted on the same side as the jacks, opposite the other components.

These were corrected after the first run.

# Build

There's nothing exotic about this build. Proceed as usual.

Pins 1 and 2 (counterclockwise and wiper pins as viewed from front) of the Clock Rate pot should be connected together, and pins 2 and 3 should be wired to the PCB via Molex connectors or soldered directly. All three pins of the Signal Level pot should be wired to the PCB. Mount the S&H/T&H switch horizontally, and then the left and center pins (again as viewed from front) should be wired to the PCB. See labels on the PCB indicating which pin goes to which point (noting Erratum above).
