---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd23d749cdccab697e34cb7973c44e76193bab25
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085906"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TabsRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
    Filter: "teamsApp/id%20eq%20'com.microsoft.teamspace.tab.planner'",
}
options := &msgraphsdk.TabsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Tabs().Get(options)


```