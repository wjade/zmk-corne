# Armno's ZMK firmware

ZMK firware for my Corne wireless split keyboard.

Steps to update the keymaps (A note to myself. I always forget this.)

- Make changes in `corne.keymap` using [Keymap Editor](https://nickcoutsos.github.io/keymap-editor/) and push to github
- Wait for [GitHub Actions](https://github.com/armno/zmk-config/actions) to finish the build. Then download the artifacts.
- Connect the left keyboard to the computur via USB. **Use a proper USB-C cable** and not the magnetic one.
- Use a tweezer to short circuit `RST` and `GND` pins. When success, there should be a storage drive named `NICENANO` shows up in the Finder.
- Copy the left firmware to the NICENANO storage. When success, the storage will be automatically unmounted.
- Repeat steps for the right keyboard.

![pins](./pins.jpg)

### 2 parts unable to pair

Most likely I'll need to fix it with the reset firmware. See https://zmk.dev/docs/troubleshooting#split-keyboard-halves-unable-to-pair

The left keyboard's switch is also not very good. Better leave if on all the time.
