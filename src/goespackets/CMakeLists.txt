add_executable(goespackets goespackets.cc options.cc)
add_sanitizers(goespackets)
install(TARGETS goespackets COMPONENT goestools RUNTIME DESTINATION bin)
target_link_libraries(goespackets nanomsg packet_reader packet_writer util m stdc++)
