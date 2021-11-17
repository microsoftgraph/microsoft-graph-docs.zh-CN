---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e04433e728ba6389c75afe4ef4d43ab55410b57f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984960"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetInputIds( []String {
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}",
}
sourceIdType := "restId"
requestBody.SetSourceIdType(&sourceIdType)
targetIdType := "restImmutableEntryId"
requestBody.SetTargetIdType(&targetIdType)
options := &msgraphsdk.TranslateExchangeIdsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Me().TranslateExchangeIds().Post(options)


```