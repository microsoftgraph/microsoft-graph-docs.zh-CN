---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 37379cc447a3a548a6c825e88b30e0c16160bfa1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347339"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Quality = @{
        "@odata.type" = "#microsoft.graph.teleconferenceDeviceQuality"
        CallChainId = "0622673d-9f69-49b3-9d4f-5ec64f42ecce"
        ParticipantId = "ea078406-b5d4-4d3c-b85e-90103dcec7f6"
        MediaLegId = "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f"
        DeviceName = "TestAgent"
        DeviceDescription = "TestDescription"
        MediaQualityList = @(
            @{
                "@odata.type" = "#microsoft.graph.teleconferenceDeviceAudioQuality"
                ChannelIndex = 1
                MediaDuration = "PT20M"
                NetworkLinkSpeedInBytes = 13000
                LocalIPAddress = "127.0.0.1"
                LocalPort = 6300
                RemoteIPAddress = "102.1.1.101"
                RemotePort = 6301
                InboundPackets = 5500
                OutboundPackets = 5400
                AverageInboundPacketLossRateInPercentage = 0.01
                AverageOutboundPacketLossRateInPercentage = 0.02
                MaximumInboundPacketLossRateInPercentage = 0.05
                MaximumOutboundPacketLossRateInPercentage = 0.06
                AverageInboundRoundTripDelay = "PT0.03S"
                AverageOutboundRoundTripDelay = "PT0.04S"
                MaximumInboundRoundTripDelay = "PT0.13S"
                MaximumOutboundRoundTripDelay = "PT0.14S"
                AverageInboundJitter = "PT0.01S"
                AverageOutboundJitter = "PT0.015S"
                MaximumInboundJitter = "PT0.023S"
                MaximumOutboundJitter = "PT0.024S"
            }
            @{
                "@odata.type" = "#microsoft.graph.teleconferenceDeviceVideoQuality"
                ChannelIndex = 1
                MediaDuration = "PT20M"
                NetworkLinkSpeedInBytes = 13000
                LocalIPAddress = "127.0.0.1"
                LocalPort = 6300
                RemoteIPAddress = "102.1.1.101"
                RemotePort = 6301
                InboundPackets = 5500
                OutboundPackets = 5400
                AverageInboundPacketLossRateInPercentage = 0.01
                AverageOutboundPacketLossRateInPercentage = 0.02
                MaximumInboundPacketLossRateInPercentage = 0.05
                MaximumOutboundPacketLossRateInPercentage = 0.06
                AverageInboundRoundTripDelay = "PT0.03S"
                AverageOutboundRoundTripDelay = "PT0.04S"
                MaximumInboundRoundTripDelay = "PT0.13S"
                MaximumOutboundRoundTripDelay = "PT0.14S"
                AverageInboundJitter = "PT0.01S"
                AverageOutboundJitter = "PT0.015S"
                MaximumInboundJitter = "PT0.023S"
                MaximumOutboundJitter = "PT0.024S"
            }
            @{
                "@odata.type" = "#microsoft.graph.teleconferenceDeviceScreenSharingQuality"
                ChannelIndex = 1
                MediaDuration = "PT20M"
                NetworkLinkSpeedInBytes = 13000
                LocalIPAddress = "127.0.0.1"
                LocalPort = 6300
                RemoteIPAddress = "102.1.1.101"
                RemotePort = 6301
                InboundPackets = 5500
                OutboundPackets = 5400
                AverageInboundPacketLossRateInPercentage = 0.01
                AverageOutboundPacketLossRateInPercentage = 0.02
                MaximumInboundPacketLossRateInPercentage = 0.05
                MaximumOutboundPacketLossRateInPercentage = 0.06
                AverageInboundRoundTripDelay = "PT0.03S"
                AverageOutboundRoundTripDelay = "PT0.04S"
                MaximumInboundRoundTripDelay = "PT0.13S"
                MaximumOutboundRoundTripDelay = "PT0.14S"
                AverageInboundJitter = "PT0.01S"
                AverageOutboundJitter = "PT0.015S"
                MaximumInboundJitter = "PT0.023S"
                MaximumOutboundJitter = "PT0.024S"
            }
        )
    }
}

Invoke-MgLogCommunicationCallTeleconferenceDeviceQuality -BodyParameter $params

```