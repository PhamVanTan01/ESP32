


# RGB LED Control

This project demonstrates how to control an RGB LED using an ESP32. The LED can display different colors based on specific events or states.

## Hardware Setup

1. Connect the RGB LED to the following GPIO pins on the ESP32:
   - Red: GPIO 21
   - Green: GPIO 22
   - Blue: GPIO 23

## Software Configuration

1. Make sure you have the ESP-IDF (Espressif IoT Development Framework) installed.
2. Include the `rgb_led.h` and `rgb_led.c` files in your project.
3. Initialize the RGB LED settings using `rgb_led_pwm_init()` function.
4. Set the desired color using `rgb_led_set_color(red, green, blue)` function.

## Example Usage

### WiFi Application Started

```c
#include "rgb_led.h"

void app_main(void)
{
    // Initialize WiFi and other components
    // ...

    // Indicate WiFi application started
    rgb_led_wifi_app_started();

    // Other tasks
    // ...
}

HTTP Server Started
#include "rgb_led.h"

void app_main(void)
{
    // Initialize HTTP server and other components
    // ...

    // Indicate HTTP server started
    rgb_led_http_server_started();

    // Other tasks
    // ...
}

WiFi Connected
#include "rgb_led.h"

void app_main(void)
{
    // Connect to WiFi
    // ...

    // Indicate WiFi connected
    rgb_led_wifi_connected();

    // Other tasks
    // ...
}

Remember to adjust the color values (0-255) according to your preference. Feel free to modify the code to suit your specific use case!
Author: Teo


Feel free to customize the content as needed. If you have any further questions or need additional assistance, feel free to ask! 😊

