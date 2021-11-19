---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce3f2eaad9a9f21e0b3a9526564783430772031c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChannelRequestBuilderGetQueryParameters{
    Filter: "lastModifiedDateTime%20gt%202019-11-01T00:00:00Z%20and%20lastModifiedDateTime%20lt%202021-11-01T00:00:00Z",
}
options := &msgraphsdk.ChannelRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Get(options)


```