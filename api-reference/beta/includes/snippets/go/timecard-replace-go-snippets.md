---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 348f0bb1a2452457df696484b3736a317b0b09ba
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104117"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "userId": "70e47528-2fae-42b5-9d8e-ee73ccd90603",
    "state": "clockedOut",
    "confirmedBy": "None",
    "notes": nil,
    "breaks":  []Object {
    }
}
options := &msgraphsdk.TimeCardRequestBuilderPutOptions{
    Body: requestBody,
}
teamId := "team-id"
timeCardId := "timeCard-id"
graphClient.TeamsById(&teamId).Schedule().TimeCardsById(&timeCardId).Put(options)


```