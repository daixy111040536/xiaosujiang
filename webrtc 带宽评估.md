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
RTCPReceiver::TriggerCallbacksFromRTCPPacket(关键结构体rtcp_packet_information（RTCPReceiver::IncomingRTCPPacket填充）)


RTCPReceiver::TriggerCallbacksFromRTCPPacket 内有两个分支

一个处理kRtcpRemb：
BitrateControllerImpl::OnReceivedEstimatedBitrate
SendSideBandwidthEstimation::UpdateReceiverEstimate
SendSideBandwidthEstimation::CapBitrateToThresholds(
修改
)
一个处理kRtcpRr





```