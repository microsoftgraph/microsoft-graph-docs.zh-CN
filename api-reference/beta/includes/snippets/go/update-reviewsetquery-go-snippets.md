---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e75daa7c3ab0992d9296d78a5ad5f6d2514dfb3b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091051"
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
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).Patch(options)


```