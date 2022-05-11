---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8ef93c81f2f2d655322f0920220197789e8266d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328506"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetTagsToAdd( []Tag {
    msgraphsdk.NewTag(),
    SetAdditionalData(map[string]interface{}{
        "id": "b4798d14-748d-468e-a1ec-96a2b1d49677",
    }
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).ApplyTags(case-id, reviewSet-id, reviewSetQuery-id).Post(requestBody)


```