# ASR_TTS_Tool_UE5

Capture microphone audio for ASR,play audio stream from TTS.

By using this plugin, real-time microphone audio data can be obtained, which can be sent to the ASR server for speech recognition, and the audio stream obtained from the TTS service can be played in real-time.

# ASR

First, you need to add following lines to `DefaultEngine.ini` of the project.
```
[Voice]
bEnabled = True
[SystemSettings]
voice.SilenceDetectionThreshold = -1
voice.MicNoiseGateThreshold = -1
```

![](UE5/ASR1.png)
![](UE5/ASR2.png)
![](UE5/ASR3.png)
![](UE5/ASR4.png)

# TTS

![](UE5/TTS1.png)
![](UE5/TTS2.png)
![](UE5/TTS3.png)
