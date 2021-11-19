---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc91690d4649ae2eb84aded5280b4b9b0e1bac08
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'private'",
}
options := &msgraphsdk.ChannelsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Get(options)


```