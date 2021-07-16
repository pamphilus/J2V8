project(j2v8_jni)
cmake_minimum_required(VERSION 3.6)
set(CMAKE_CXX_STANDARD 14)
set(CMAKE_VERBOSE_MAKEFILE ON)

add_executable(j2v8_jni com_eclipsesource_v8_V8Impl.cpp)


include_directories(
    /home/elmi/EclipseSource/J2V8/v8.out/include
    /usr/lib/jvm/java-8-openjdk/include
    /usr/lib/jvm/java-8-openjdk/include/linux
)
set(src_files
    com_eclipsesource_v8_V8Impl.cpp
    com_eclipsesource_v8_V8Impl.h
)

source_group("" FILES ${src_files})

include_directories(${include_dirs})
