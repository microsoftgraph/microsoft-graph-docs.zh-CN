---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c94fc8e25612a309a9cb4662acbd6bf7776328b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102841"
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
options := &msgraphsdk.LegalHoldsRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).LegalHolds().Post(options)


```