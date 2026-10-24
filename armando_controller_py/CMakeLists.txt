cmake_minimum_required(VERSION 3.8)
project(armando_controller_py)

find_package(ament_cmake REQUIRED)

install(
  PROGRAMS scripts/armando_keyboard_teleop.py
  DESTINATION lib/${PROJECT_NAME}
)

if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)
  ament_lint_auto_find_test_dependencies()
endif()

ament_package()
