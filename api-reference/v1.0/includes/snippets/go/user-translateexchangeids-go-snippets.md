---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55d8e9a451c4c4f64e9e6a3eb0585cd84cf89733
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327734"
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
result, err := graphClient.Me().TranslateExchangeIds().Post(requestBody)


```