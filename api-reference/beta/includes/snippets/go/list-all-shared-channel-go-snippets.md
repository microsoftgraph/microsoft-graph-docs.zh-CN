---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4c82d13853a048d261073abfeef35314ab39bb5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212528"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AllChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'shared'",
}
options := &msgraphsdk.AllChannelsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).AllChannels().Get(options)


```