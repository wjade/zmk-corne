# Armno's ZMK firmware

ZMK firware for my Corne wireless split keyboard.

To udpate to keymaps (which I always forget):

- Make changes in `corne.keymap` and push to github
- Wait for [GitHub Actions](https://github.com/armno/zmk-config/actions) to finish the build. Then download the artifacts.
- Connect the left keyboard to the computur via USB
- Use a tweezer to short circuit RST and GND pins. When success, there should be a storage drive named NICENANO shows up in the Finder.
- Copy the left firmware to the NICENANO storage. When success, the storage will be automatically unmounted.
- Repeat steps for the right keyboard.
