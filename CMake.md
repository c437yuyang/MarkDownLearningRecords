#linux下 最简单的hello world的生成方法
* mkdir ${projectname}
* cd ${projectname}
* vim xxx.cpp
* vim CMakeLists.txt
* 内容:

	project(hello)

	cmake_minimum_required(VERSION 2.8)
	
	aux_source_directory(. DIR_SRCS)
	
	add_executable(hello ${DIR_SRCS})
> http://blog.csdn.net/fan_hai_ping/article/details/42524205 这里有基本的命令解释


* mkdir build
* cd build
* cmake ..
* make