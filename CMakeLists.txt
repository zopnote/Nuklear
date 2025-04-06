cmake_minimum_required(VERSION 3.16)
project(Nuklear VERSION 4.12.6)
set(CMAKE_C_STANDARD 90)
add_library(Nuklear STATIC)

target_compile_definitions(Nuklear PRIVATE NK_IMPLEMENTATION)
target_precompile_headers(Nuklear PRIVATE src/nuklear.h)
target_precompile_headers(Nuklear PRIVATE src/nuklear_internal.h)

target_sources(Nuklear PRIVATE
        src/nuklear_9slice.c
        src/nuklear_buffer.c
        src/nuklear_button.c
        src/nuklear_chart.c
        src/nuklear_color.c
        src/nuklear_color_picker.c
        src/nuklear_combo.c
        src/nuklear_context.c
        src/nuklear_contextual.c
        src/nuklear_draw.c
        src/nuklear_edit.c
        src/nuklear_font.c
        src/nuklear_group.c
        src/nuklear_image.c
        src/nuklear_input.c
        src/nuklear_knob.c
        src/nuklear_layout.c
        src/nuklear_list_view.c
        src/nuklear_math.c
        src/nuklear_menu.c
        src/nuklear_page_element.c
        src/nuklear_panel.c
        src/nuklear_pool.c
        src/nuklear_popup.c
        src/nuklear_progress.c
        src/nuklear_property.c
        src/nuklear_scrollbar.c
        src/nuklear_selectable.c
        src/nuklear_slider.c
        src/nuklear_string.c
        src/nuklear_window.c
        src/nuklear_widget.c
        src/nuklear_vertex.c
        src/nuklear_util.c
        src/nuklear_utf8.c
        src/nuklear_tree.c
        src/nuklear_tooltip.c
        src/nuklear_toggle.c
        src/nuklear_text.c
        src/nuklear_text_editor.c
        src/nuklear_table.c
        src/nuklear_style.c
)