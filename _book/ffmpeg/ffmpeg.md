1. window使用FFmpeg录像与录音（内录），使用dshow录制

   * `ffmpeg -list_devices true -f dshow -i dummy`   列出可用的录制设备

   * `ffmpeg -f dshow -i video="Camera":audio="Microphone" outfile` 录像与录音，其中Camera为视频设备名，Microphone为音频设备名

   * 如果没有录制声卡的设备，安装Screen Capturer Recorder软件，[项目地址](https://sourceforge.net/projects/screencapturer/files/) ,安装后再列出可用的录制设备,可看见如下设备

     ```shell
     DirectShow video devices (some may be both video and audio devices)
     “screen-capture-recorder”    //视频设备
     DirectShow audio devices
     “virtual-audio-capturer”  //音频设备
     ```

     

2. window使用FFmpeg录制并hls点播

   * `ffmpeg -f dshow -i video="Camera":audio="Microphone" fileName.m3u8`  录制，并输出到http服务所在目录
   * 搭建http服务器

3. 
