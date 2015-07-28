cmake_minimum_required (VERSION 2.8.11)
project (online-random-forest)
add_executable( online-random-forest
  src/classifier.cpp
  src/data.cpp
  src/hyperparameters.cpp
  src/Online-Forest.cpp
  src/onlinenode.cpp
  src/onlinerf.cpp
  src/onlinetree.cpp
  src/randomtest.cpp
  src/utilities.cpp
)

target_link_libraries( online-random-forest
  atlas
  lapack
  config++
  blas
)