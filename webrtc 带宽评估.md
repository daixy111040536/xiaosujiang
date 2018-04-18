---
title: webrtc 带宽评估
tags: webrtc，带宽评估
grammar_cjkRuby: true
---


# 代码跟踪
```c++?linenums
UdpTransportImpl::IncomingRTCPCallback
UdpTransportImpl::IncomingRTCPFunction
VoiceChannelTransport::IncomingRTCPPacket
Channel::ReceivedRTCPPacket

VideoSendStream::DeliverRtcp
ModuleRtpRtcpImpl::IncomingRtcpPacket
RTCPReceiver::TriggerCallbacksFromRTCPPacket(关键结构体rtcp_packet_information)




```