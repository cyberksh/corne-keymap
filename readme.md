# KeyMap

Didn't push the complete qmk repo because too many files.

Copy over the files to:

`qmk_firmware/keyboards/crkbd/keymaps/cyberksh/`

Test code:

`qmk compile -kb crkbd -km cyberksh -e CONVERT_TO=promicro_rp2040`

Flash code:

Connect each side with the usb cable and double press reset button
to go into flash mode.

`qmk flash -kb crkbd -km cyberksh -e CONVERT_TO=promicro_rp2040`

