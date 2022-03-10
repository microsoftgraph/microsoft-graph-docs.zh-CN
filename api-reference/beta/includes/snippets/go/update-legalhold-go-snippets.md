---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed90257cd3cc8913a02b01e8058d9c42b071f4f1
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412593"
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
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).Patch(options)


```