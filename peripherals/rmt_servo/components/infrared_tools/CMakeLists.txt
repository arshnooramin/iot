set(component_srcs "src/ir_builder_rmt_nec.c"
                   "src/ir_builder_rmt_rc5.c"
                   "src/ir_parser_rmt_nec.c"
                   "src/ir_parser_rmt_rc5.c"
                   "src/led_strip_rmt_ws2812.c")

idf_component_register(SRCS "${component_srcs}"
                       INCLUDE_DIRS "include"
                       PRIV_INCLUDE_DIRS ""
                       PRIV_REQUIRES "driver"
                       REQUIRES "")
