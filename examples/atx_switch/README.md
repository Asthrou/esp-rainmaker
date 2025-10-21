# ATX Switch Example

## Build and Flash firmware

Follow the ESP RainMaker Documentation [Get Started](https://rainmaker.espressif.com/docs/get-started.html) section to build and flash this firmware. Just note the path of this example.

## What to expect in this example?

- This example uses the BOOT button and LED on the ELEGOO ESP-WROOM-32/DOIT ESP32 DEVKIT V1 Development Board to demonstrate a switch.
- The LED state (Onboard Pin 2) indicates the state of the switch.
- Pressing the BOOT button will toggle the state of the switch and hence the LED. This will also reflect on the phone app.
- Toggling the button on the phone app should toggle the LED on your board, and also print messages like these on the ESP32 monitor:

```
I (16073) app_main: Received value = true for Switch - power
```

### LED not working?

The ELEGOO ESP-WROOM-32/DOIT ESP32 DEVKIT V1 boards has the LED connected to GPIO 2. However, other boards may have it on another GPIO. Please use `CONFIG_WS2812_LED_GPIO` to set the appropriate value.

### Reset to Factory

Press and hold the BOOT button for more than 3 seconds to reset the board to factory defaults. You will have to provision the board again to use it.


### Reference:
ELEGOO ESP-WROOM-32/DOIT ESP32 DEVKIT V1 Development Board:
https://www.espboards.dev/esp32/esp32doit-devkit-v1/