---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055da56912a8a2b752526d1b29150e10b616f62a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092440"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChatMessageRequestBuilderGetQueryParameters{
    Deltatoken: "aQdvS1VwGCSRxVmZJqykmDik_JIC44iCZpv-GLiA2VnFuE5yG-kCEBROb2iaPT_y_eMWVQtBO_ejzzyIxl00ji-tQ3HzAbW4liZAVG88lO3nG_6-MBFoHY1n8y21YUzjocG-Cn1tCNeeLPLTzIe5Dw.EP9gLiCoF2CE_e6l_m1bTk2aokD9KcgfgfcLGqd1r_4",
}
options := &msgraphsdk.ChatMessageRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
channelId := "channel-id"
chatMessageId := "chatMessage-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).MessagesById(&chatMessageId).Get(options)


```