add_executable(straight straight.cpp)

target_link_libraries(straight 
    pico_stdlib
    hardware_gpio
    hardware_pwm
    kaguya-pin
    #motor_encoder
    umotor
)


pico_enable_stdio_usb(straight 1)
pico_enable_stdio_uart(straight 0)

pico_add_extra_outputs(straight)
