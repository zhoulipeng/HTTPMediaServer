# HTTPMediaServer
Simple http media server software
# 目标

* 一、在开源的srs(simpe rtmp server)的基础上构建软件，保持简洁性，而且要做到更简洁
* 二、支持主流的推流格式，如，rtmp, httpflv, ts
* 三、利用chunk编码做传输层，用http chunk-extension 定义的视频传输层表示协议，简化传输解析
* 四、远景目标支持4k高清， MPEG-H MMT传输协议的应用 
* 五、html5 交互式直播服务
# 使用 HTTP chunk extension 表示传输的媒体信息
* 视频编码表示：
   * ;vc=264|265|vp9
* 音频编码编码表示：
   * ;ac=aac|mp3
* 视频帧率表示：
   * ;vfr=29.97
* 表示视频图像组（Group of pictures）开始：
   * ;gop
