---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 935e5d39e8805b0f923b2df854fa4311e4e3e6f1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUserSource()
email := "adelev@contoso.com"
requestBody.SetEmail(&email)
includedSources := "mailbox"
requestBody.SetIncludedSources(&includedSources)
caseId := "case-id"
legalHoldId := "legalHold-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).UserSources().Post(requestBody)


```