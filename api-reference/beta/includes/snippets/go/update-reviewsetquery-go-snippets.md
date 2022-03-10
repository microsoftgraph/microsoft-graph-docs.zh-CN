---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24b3ac4f4e20a485a07710bc7bd930add3ed2e9c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411667"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewReviewSetQuery()
displayName := "My Query 1 - Renamed"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ReviewSetQueryRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).Patch(options)


```