include_directories(./ffmpeg_base)

macro(target_link_ffmpeg_base name)
    message("${name} link ffmpeg_base")
    target_link_libraries(${name}
            ffmpeg_base
            )
endmacro()

add_subdirectory(ffmpeg_base)
add_subdirectory(ffmpeg_00_run_ffplay)
add_subdirectory(ffmpeg_01_print_log)
add_subdirectory(ffmpeg_02_file_info)
add_subdirectory(ffmpeg_03_open_codec)
add_subdirectory(ffmpeg_04_decode_video)

