cmake_minimum_required(VERSION 3.26)
project(myrtsp C)

set(CMAKE_C_STANDARD 11)

include_directories(.)
include_directories(rtsp_lib)

add_executable(myrtsp
        rtsp_lib/comm.h
        rtsp_lib/queue.h
        rtsp_lib/rtp_enc.c
        rtsp_lib/rtp_enc.h
        rtsp_lib/rtsp_demo.c
        rtsp_lib/rtsp_demo.h
        rtsp_lib/rtsp_msg.c
        rtsp_lib/rtsp_msg.h
        rtsp_lib/stream_queue.c
        rtsp_lib/stream_queue.h
        rtsp_lib/test.c
        rtsp_lib/utils.c
        rtsp_lib/utils.h
        smp/sample_rtsp.c
        sample_comm_venc.c
        sample_rtsp.h
        sample_rtsp_main.c)
