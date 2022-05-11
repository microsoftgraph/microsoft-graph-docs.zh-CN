---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5061ffbd9c8db51fcf16c2a99561ea88d4b79ea
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326924"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHolds().Post(requestBody)


```