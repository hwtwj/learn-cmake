PROJECT(HELLO)
ADD_SUBDIRECTORY(src bin)
INSTALL(FILES COPYRIGHT README DESTINATION share/doc/cmake/practice2)
INSTALL(PROGRAMS ${PROJECT_BINARY_DIR}/bin/hello runhello.sh DESTINATION bin)
INSTALL(DIRECTORY doc/ DESTINATION share/doc/cmake/practice2)
