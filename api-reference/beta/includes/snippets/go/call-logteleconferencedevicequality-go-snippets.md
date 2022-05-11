---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d115c3175cf5fe6da71a8f099aec67563af0e8f2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328307"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewQualityRequestBody()
quality := msgraphsdk.NewTeleconferenceDeviceQuality()
requestBody.SetQuality(quality)
callChainId := "0622673d-9f69-49b3-9d4f-5ec64f42ecce"
quality.SetCallChainId(&callChainId)
participantId := "ea078406-b5d4-4d3c-b85e-90103dcec7f6"
quality.SetParticipantId(&participantId)
mediaLegId := "bd9ee398-4b9d-42c7-8b8d-4e8efad9435f"
quality.SetMediaLegId(&mediaLegId)
deviceName := "TestAgent"
quality.SetDeviceName(&deviceName)
deviceDescription := "TestDescription"
quality.SetDeviceDescription(&deviceDescription)
quality.SetMediaQualityList( []TeleconferenceDeviceMediaQuality {
    msgraphsdk.NewTeleconferenceDeviceMediaQuality(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.teleconferenceDeviceAudioQuality",
        "channelIndex": ,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": ,
        "localIPAddress": "127.0.0.1",
        "localPort": ,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": ,
        "inboundPackets": ,
        "outboundPackets": ,
        "averageInboundPacketLossRateInPercentage": ,
        "averageOutboundPacketLossRateInPercentage": ,
        "maximumInboundPacketLossRateInPercentage": ,
        "maximumOutboundPacketLossRateInPercentage": ,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S",
    }
    msgraphsdk.NewTeleconferenceDeviceMediaQuality(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.teleconferenceDeviceVideoQuality",
        "channelIndex": ,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": ,
        "localIPAddress": "127.0.0.1",
        "localPort": ,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": ,
        "inboundPackets": ,
        "outboundPackets": ,
        "averageInboundPacketLossRateInPercentage": ,
        "averageOutboundPacketLossRateInPercentage": ,
        "maximumInboundPacketLossRateInPercentage": ,
        "maximumOutboundPacketLossRateInPercentage": ,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S",
    }
    msgraphsdk.NewTeleconferenceDeviceMediaQuality(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
        "channelIndex": ,
        "mediaDuration": "PT20M",
        "networkLinkSpeedInBytes": ,
        "localIPAddress": "127.0.0.1",
        "localPort": ,
        "remoteIPAddress": "102.1.1.101",
        "remotePort": ,
        "inboundPackets": ,
        "outboundPackets": ,
        "averageInboundPacketLossRateInPercentage": ,
        "averageOutboundPacketLossRateInPercentage": ,
        "maximumInboundPacketLossRateInPercentage": ,
        "maximumOutboundPacketLossRateInPercentage": ,
        "averageInboundRoundTripDelay": "PT0.03S",
        "averageOutboundRoundTripDelay": "PT0.04S",
        "maximumInboundRoundTripDelay": "PT0.13S",
        "maximumOutboundRoundTripDelay": "PT0.14S",
        "averageInboundJitter": "PT0.01S",
        "averageOutboundJitter": "PT0.015S",
        "maximumInboundJitter": "PT0.023S",
        "maximumOutboundJitter": "PT0.024S",
    }
}
quality.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.teleconferenceDeviceQuality",
}
graphClient.Communications().Calls().LogTeleconferenceDeviceQuality().Post(requestBody)


```