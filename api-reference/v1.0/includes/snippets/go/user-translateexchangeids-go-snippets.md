---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e600fbce27644d876b1d0ca010d7713ed82307c6
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098128"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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