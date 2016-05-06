# GPIO

---

### enum gpio_mode

```c
enum gpio_mode {
        LS_SHARED,
        LS_GREEDY,
        LS_WEAK,
}
```

### libsoc_gpio_request
```c
gpio *libsoc_gpio_request(unsigned int gpio_id, enum gpio_mode mode)
```

Request a GPIO by it's Linux ID number and set the [gpio_mode](#enum-gpio_mode)
under which libsoc will hold the file descriptor.

```c
#define MY_PIN_ID 65

my_pin = libsoc_gpio_request(MY_PIN_ID, LS_SHARED);
```

### libsoc_gpio_request
```c
`gpio *libsoc_gpio_request(unsigned int gpio_id, enum gpio_mode mode)`
```

# SPI
# I2C
# PWM
