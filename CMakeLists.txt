add_library(mbed-blackpill-f401cc INTERFACE)

target_sources(mbed-blackpill-f401cc
    INTERFACE
        PeripheralPins.c
        system_clock.c
)

target_include_directories(mbed-blackpill-f401cc
    INTERFACE
        .
)

target_link_libraries(mbed-blackpill-f401cc INTERFACE mbed-stm32f401xc)
