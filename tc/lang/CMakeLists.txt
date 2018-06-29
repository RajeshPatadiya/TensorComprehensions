
add_library(
  tc_lang

  SHARED

  error_report.cc
  parser.cc
  lexer.cc
  tc_format.cc
)

target_link_libraries(
  tc_lang

  gflags)

install(
  TARGETS
  tc_lang

  DESTINATION lib
)
