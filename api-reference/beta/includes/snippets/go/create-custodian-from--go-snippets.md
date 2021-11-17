---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8c008c98591bbf771e58e2fb4dc39a1f01d8f53
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023917"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewCustodian()
email := "AdeleV@contoso.com"
requestBody.SetEmail(&email)
applyHoldToSources := "true"
requestBody.SetApplyHoldToSources(&applyHoldToSources)
options := &msgraphsdk.CustodiansRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).Custodians().Post(options)


```