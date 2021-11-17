---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e8a3971bc5230064e7dc29d84f207bf0bab6008
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986697"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewLegalHold()
description := "This is a description for a legalHold"
requestBody.SetDescription(&description)
options := &msgraphsdk.LegalHoldRequestBuilderPatchOptions{
    Body: requestBody,
}
caseId := "case-id"
legalHoldId := "legalHold-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).Patch(options)


```