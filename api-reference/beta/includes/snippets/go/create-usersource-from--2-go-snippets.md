---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afd9ff2d5447562addbb858186f08e298919822e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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