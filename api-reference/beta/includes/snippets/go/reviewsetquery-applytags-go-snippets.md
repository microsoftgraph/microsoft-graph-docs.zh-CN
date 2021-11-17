---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8751632b0f4e2afa9497433cfcaff7a0091f4e80
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986669"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetTagsToAdd( []Tag {
    msgraphsdk.NewTag(),
    SetAdditionalData(map[string]interface{}{
        "id": "b4798d14-748d-468e-a1ec-96a2b1d49677",
    }
}
options := &msgraphsdk.ApplyTagsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
reviewSetId := "reviewSet-id"
reviewSetQueryId := "reviewSetQuery-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).ReviewSetsById(&reviewSetId).QueriesById(&reviewSetQueryId).ApplyTags().Post(options)


```