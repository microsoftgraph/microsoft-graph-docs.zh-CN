---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1e35094bbfc9e835873e617336f6eb304ff5d36
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020970"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewLegalHold()
description := "String"
requestBody.SetDescription(&description)
createdBy := msgraphsdk.NewIdentitySet()
requestBody.SetCreatedBy(createdBy)
createdBy.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.identitySet",
}
isEnabled := "Boolean"
requestBody.SetIsEnabled(&isEnabled)
status := "String"
requestBody.SetStatus(&status)
contentQuery := "String"
requestBody.SetContentQuery(&contentQuery)
requestBody.SetErrors( []String {
    "String",
}
displayName := "String"
requestBody.SetDisplayName(&displayName)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.ediscovery.legalHold",
}
options := &msgraphsdk.LegalHoldsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHolds().Post(options)


```