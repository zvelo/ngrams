CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(ngrams)

SET(SOURCES
  string.cpp
  INgrams.cpp
  ngrams.cpp
  CharNgrams.cpp
  WordNgrams.cpp
  text2wfreq.cpp
)

SET(HEADERS
  mystring.h
  INgrams.h
  ngrams.h
  CharNgrams.h
  WordNgrams.h
  text2wfreq.h
  ternarySearchTree.h
  config.h
  vector.h
)

ADD_LIBRARY(ngrams SHARED ${SOURCES})

INSTALL(TARGETS ngrams DESTINATION lib)
INSTALL(FILES ${HEADERS} DESTINATION include)
