# KeyMap

Didn't push the complete qmk repo because too many files.

Copy over the files to:

`qmk_firmware/keyboards/crkbd/keymaps/cyberksh/`

Update code in `crkbd/crkbd.c`:

* Set `OLED_ROTATION_270` instead of 180
* Comment out `oled_render_logo()`

Test code:

`qmk compile -kb crkbd -km cyberksh -e CONVERT_TO=promicro_rp2040`

Flash code:

Connect each side with the usb cable and double press reset button
to go into flash mode.

`qmk flash -kb crkbd -km cyberksh -e CONVERT_TO=promicro_rp2040`

## TODOs:

* [ ] Create independent config or figure out how to reuse code 
* [ ] Check why Luna doesn't jump
* [ ] Set timeout to be 60s like the default layer
* [ ] Add more cool stuff

