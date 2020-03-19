cmake_minimum_required(VERSION 3.9)
project(muse)

set(CMAKE_CXX_STANDARD 11)

link_libraries(m)
link_libraries(z)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O0 -w -g -Wall -D_FILE_OFFSET_BITS=64 -D_LARGEFILE64_SOURCE")

add_executable(muse
        bam.cpp
        bam.h
        bam_supplement.cpp
        bgzf.c
        bgzf.h
        faidx.c
        faidx.h
        fet.cpp
        index.c
        khash.h
        kprobaln.c
        kprobaln.h
        kseq.h
        ksort.h
        kstring.c
        kstring.h
        MuSE.cpp
        razf.c
        razf.h
        sample.cpp
        sample.h
        tabix.h)
