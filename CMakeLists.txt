CMAKE_MINIMUM_REQUIRED(VERSION 2.6 FATAL_ERROR)
CMAKE_POLICY(VERSION 2.6)

INCLUDE(${CMAKE_INSTALL_PREFIX}/share/cmake/torch/TorchConfig.cmake)

SET(src)
SET(luasrc init.lua OptionParser.lua Profiler.lua)

ADD_TORCH_PACKAGE(xlua "${src}" "${luasrc}" "System")

