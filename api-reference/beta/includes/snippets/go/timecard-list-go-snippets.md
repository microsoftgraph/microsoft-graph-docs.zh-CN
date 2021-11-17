---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 119ea8ad2c69dfc14750fef0989b12bd78058cac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60989154"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.TimeCardsRequestBuilderGetQueryParameters{
    Top: 2,
    Filter: "state%20eq%20'clockedOut'",
}
options := &msgraphsdk.TimeCardsRequestBuilderGetOptions{
    Q: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().TimeCards().Get(options)


```