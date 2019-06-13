## build janus

    docker build -t alexwoo/janus ./

## run janus

	docker run --rm -p 8188:8188 alexwoo/janus


## janus安装特殊说明

由于目需要使用janus提供的基于录制的后处理janus-pp-rec能力,该能力需要基于ffmpeg的依赖库, 因此需要在安装janus前, 优先编译ffmpeg, 并设置好相应的环境变量.
