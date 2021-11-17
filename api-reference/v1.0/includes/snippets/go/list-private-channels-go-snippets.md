---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 191de1e24a2a3a88bdc540d212c85601299498c0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988629"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.ChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'private'",
}
options := &msgraphsdk.ChannelsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Get(options)


```