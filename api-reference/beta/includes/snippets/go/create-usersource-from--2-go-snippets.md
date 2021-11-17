---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e609cff69c86169cd383d4efb82d19f6721e0c04
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986718"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUserSource()
email := "adelev@contoso.com"
requestBody.SetEmail(&email)
includedSources := "mailbox"
requestBody.SetIncludedSources(&includedSources)
options := &msgraphsdk.UserSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
legalHoldId := "legalHold-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHoldsById(&legalHoldId).UserSources().Post(options)


```