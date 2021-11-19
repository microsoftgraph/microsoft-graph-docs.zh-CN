---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f33cb2b3331141bfa9a116c1b3ff61271aa61af1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092868"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTemporaryAccessPassAuthenticationMethod()
startDateTime, err := time.Parse(time.RFC3339, "2021-01-26T00:00:00.000Z")
requestBody.SetStartDateTime(&startDateTime)
lifetimeInMinutes := int32(60)
requestBody.SetLifetimeInMinutes(&lifetimeInMinutes)
isUsableOnce := false
requestBody.SetIsUsableOnce(&isUsableOnce)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
}
options := &msgraphsdk.TemporaryAccessPassMethodsRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethods().Post(options)


```