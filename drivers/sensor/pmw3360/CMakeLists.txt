zephyr_library_amend()

zephyr_library_sources_ifdef(CONFIG_SENSOR_PMW3350  pmw3360.c)

target_sources_ifdef(CONFIG_ZMK_SENSOR_PMW3360_IDLE_SLEEPER app PRIVATE pmw3360_priv.c)
