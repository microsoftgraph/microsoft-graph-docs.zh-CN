---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98e5e5b8c51a4194d9d68e94963dd07b5175ea5d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103128"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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