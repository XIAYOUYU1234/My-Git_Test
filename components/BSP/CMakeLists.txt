set(src_dirs
            POWER
            KEY
            I2C
            USART
            XL9555
            CI1303)

set(include_dirs
            POWER
            KEY
            I2C
            USART
            XL9555
            CI1303)

set(requires
            driver)

idf_component_register(SRC_DIRS ${src_dirs} INCLUDE_DIRS ${include_dirs} REQUIRES ${requires})

component_compile_options(-ffast-math -O3 -Wno-error=format=-Wno-format)