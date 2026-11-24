dfhack_plugin(smooth-movement-adv smooth-movement.cpp LINK_LIBRARIES lua)
target_include_directories(smooth-movement-adv PRIVATE ${SDL2_INCLUDE_DIRS})
target_compile_features(smooth-movement-adv PRIVATE cxx_std_17)

add_executable(
    smooth-movement-adv-test
    EXCLUDE_FROM_ALL
    test_visual_animation_manager.cpp)
target_compile_features(smooth-movement-adv-test PRIVATE cxx_std_17)
