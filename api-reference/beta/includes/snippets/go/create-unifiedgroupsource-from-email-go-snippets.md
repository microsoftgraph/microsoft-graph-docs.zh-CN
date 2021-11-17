---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 54d30fe3475f81d23138c01dff0872e21e9fff76
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986923"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUnifiedGroupSource()
group := msgraphsdk.NewGroup()
requestBody.SetGroup(group)
mail := "SecretGroup@contoso.com"
group.SetMail(&mail)
includedSources := "mailbox, site"
requestBody.SetIncludedSources(&includedSources)
options := &msgraphsdk.UnifiedGroupSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
custodianId := "custodian-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).CustodiansById(&custodianId).UnifiedGroupSources().Post(options)


```