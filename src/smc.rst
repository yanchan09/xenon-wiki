##################################
System Management Controller (SMC)
##################################

The System Management Controller (SMC) is a 8051/8052 core located in
the Southbridge.

Command Map
-----------

======= =========================
Command Description
======= =========================
0x01    Get Power On Type
0x04    Get RTC
0x07    Read temps
0x0a    Get tray state
0x0f    Get AV Pack type
0x10    I2C read
0x11    (H)ANA read
0x12    Get SMC Version
0x16    Get IR address
0x17    Get Tilt Sensor
0x20    I2C write
0x21    (H)ANA write
0x82    Set Power State
0x85    Set RTC
0x88    Set Fan control algorithm
0x89    Set fan speed
0x8b    Set DVD tray
0x8c    Set power led
0x8d    Set audio mute
0x94    Set fan speed
0x95    Set IR address
0x98    Set DVD tray secure
0x99    Set ring of light
0x9a    Set RTC wake
======= =========================

.. _av_pack_types:

AV Pack Types
-------------

==== ===================
Type Description
==== ===================
0x13 HDMI + Audio
0x14 HDMI + Audio
0x1C HDMI + Audio
0x1E HDMI
0x1F HDMI
0x43 COMPOSITE - TV MODE
0x47 SCART
0x54 COMPOSITE - S-VIDEO
0x57 COMPOSITE
0x0C COMPONENT
0x0F COMPONENT
0x4F COMPOSITE HD
0x5B VGA
0x59 VGA
0x1B VGA
==== ===================

.. _register_map:

Register Map
------------

=================== ==========================
Address             Description
=================== ==========================
0x0200ea001000+0x00 Unknown
0x0200ea001000+0x04 Unknown
0x0200ea001000+0x08 Unknown
0x0200ea001000+0x0c Unknown
0x0200ea001000+0x10 [R] UART FIFO Read
0x0200ea001000+0x14 [W] UART FIFO Write
0x0200ea001000+0x18 [R] UART Status
0x0200ea001000+0x1c [R/W] UART Configuration
0x0200ea001000+0x20 Unknown
0x0200ea001000+0x24 Unknown
0x0200ea001000+0x28 Unknown
0x0200ea001000+0x2c Unknown
0x0200ea001000+0x30 Unknown
0x0200ea001000+0x34 Unknown
0x0200ea001000+0x38 Unknown
0x0200ea001000+0x3c Unknown
0x0200ea001000+0x40 Unknown
0x0200ea001000+0x44 Unknown
0x0200ea001000+0x48 Unknown
0x0200ea001000+0x4c Unknown
0x0200ea001000+0x50 Unknown
0x0200ea001000+0x54 Unknown
0x0200ea001000+0x58 Unknown
0x0200ea001000+0x5c ???: XeLL writes 0xc000000
0x0200ea001000+0x60 Unknown
0x0200ea001000+0x64 ???: XeLL writes 0x10
0x0200ea001000+0x68 Unknown
0x0200ea001000+0x6c ???: XeLL writes 0x1000000
0x0200ea001000+0x70 Unknown
0x0200ea001000+0x74 Unknown
0x0200ea001000+0x78 Unknown
0x0200ea001000+0x7c Unknown
0x0200ea001000+0x80 [W] Command FIFO Write
0x0200ea001000+0x84 [R/W] Command FIFO Status
0x0200ea001000+0x88 Unknown
0x0200ea001000+0x8c Unknown
0x0200ea001000+0x90 [R] Reply FIFO Read
0x0200ea001000+0x94 [R/W] Reply FIFO Status
0x0200ea001000+0x98 Unknown
0x0200ea001000+0x9c Unknown
0x0200ea001000+0xa0 Unknown
0x0200ea001000+0xa4 Unknown
0x0200ea001000+0xa8 Unknown
0x0200ea001000+0xac Unknown
0x0200ea001000+0xb0 Unknown
0x0200ea001000+0xb4 Unknown
0x0200ea001000+0xb8 Unknown
0x0200ea001000+0xbc Unknown
0x0200ea001000+0xc0 Unknown
0x0200ea001000+0xc4 Unknown
0x0200ea001000+0xc8 Unknown
0x0200ea001000+0xcc Unknown
0x0200ea001000+0xd0 Unknown
0x0200ea001000+0xd4 Unknown
0x0200ea001000+0xd8 Unknown
0x0200ea001000+0xdc Unknown
0x0200ea001000+0xe0 Unknown
0x0200ea001000+0xe4 Unknown
0x0200ea001000+0xe8 Unknown
0x0200ea001000+0xec Unknown
0x0200ea001000+0xf0 Unknown
0x0200ea001000+0xf4 Unknown
0x0200ea001000+0xf8 Unknown
0x0200ea001000+0xfc Unknown
=================== ==========================
