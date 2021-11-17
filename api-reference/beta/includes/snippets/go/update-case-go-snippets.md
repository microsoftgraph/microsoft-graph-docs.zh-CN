---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6b52fc6b2699b1240d387bd7cfe4289bf63731ba
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020914"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCase()
displayName := "My Case 1 - Renamed"
requestBody.SetDisplayName(&displayName)
description := "Updated description"
requestBody.SetDescription(&description)
externalId := "Updated externalId"
requestBody.SetExternalId(&externalId)
options := &msgraphsdk.CaseRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).Patch(options)


```