add_executable(complete complete.cpp)

target_link_libraries(complete cli)

add_executable(asyncsession asyncsession.cpp)

target_link_libraries(asyncsession cli)

add_executable(filesession filesession.cpp)

target_link_libraries(filesession cli)

add_executable(simplelocalsession simplelocalsession.cpp)

target_link_libraries(simplelocalsession cli)