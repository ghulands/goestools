add_executable(goeslrit goeslrit.cc options.cc)
add_sanitizers(goeslrit)
install(TARGETS goeslrit COMPONENT goestools RUNTIME DESTINATION bin)
target_link_libraries(goeslrit assembler nanomsg packet_reader m stdc++)
