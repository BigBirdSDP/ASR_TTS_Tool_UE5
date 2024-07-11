# ASR_TTS_Tool_UE5

Capture microphone audio for ASR,play audio stream from TTS.

The plugin contains an actor component, which can be attached to any actor.

![](UE5/ASR_TTS.png)

The plugin provides the functionality to capture microphone audio data which can be sent to the ASR server for speech recognition.

The plugin also provides the functionality to play the audio stream obtained from the TTS service.


# ASR Tool

First, you need to add following lines to `DefaultEngine.ini` of the project.
```
[Voice]
bEnabled = True
[SystemSettings]
voice.SilenceDetectionThreshold = -1
voice.MicNoiseGateThreshold = -1
```

初始化ASR Tool

![](UE5/ASR1.png)

开始捕获麦克风音频

![](UE5/ASR2.png)

捕获麦克风音频后，应该每0.1秒调用一次，获取有效的麦克风捕获音频数据，从而发送到ASR 服务器

![](UE5/ASR3.png)

停止捕获麦克风音频

![](UE5/ASR4.png)


# TTS Tool

初始化TTS Tool

![](UE5/TTS1.png)

设置是否自动播放音频，和是否重置音频数据

![](UE5/TTS2.png)

储存音频数据

![](UE5/TTS3.png)
