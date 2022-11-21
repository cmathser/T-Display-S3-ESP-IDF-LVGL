file(GLOB_RECURSE IMAGE_SOURCES images/*.c)


idf_component_register(SRCS "main.c" "lvgl_demo_ui.c" ${IMAGE_SOURCES}
                       INCLUDE_DIRS ".")

add_compile_definitions(LV_LVGL_H_INCLUDE_SIMPLE)
