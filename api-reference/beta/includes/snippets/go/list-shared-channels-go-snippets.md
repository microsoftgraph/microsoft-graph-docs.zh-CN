---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 999a9ff1a67d3f3892fb6f2c6daac88bfe5584ec
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'shared'",
}
options := &msgraphsdk.ChannelsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().Get(options)


```