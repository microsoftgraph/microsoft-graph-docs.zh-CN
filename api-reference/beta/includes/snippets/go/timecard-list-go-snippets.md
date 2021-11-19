---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d55e53356870367dfb6e779e8756eeec8e4d8676
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093395"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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