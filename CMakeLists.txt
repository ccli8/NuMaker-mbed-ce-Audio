# Copyright (c) 2020 ARM Limited. All rights reserved.
# SPDX-License-Identifier: Apache-2.0

add_library(nuaudio STATIC EXCLUDE_FROM_ALL)

target_include_directories(nuaudio
    PUBLIC
        .
)

target_sources(nuaudio
    PRIVATE
        I2S.cpp
        NAU88L25.cpp
        NAU8822L.cpp
)

target_link_libraries(nuaudio PUBLIC mbed-core-flags)
