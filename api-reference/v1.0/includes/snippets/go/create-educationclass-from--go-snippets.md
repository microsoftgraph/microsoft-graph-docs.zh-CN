---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 137ca3d1243c3d88bbf743f82e3b79747faab916
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327589"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
displayName := "String"
requestBody.SetDisplayName(&displayName)
mailNickname := "String"
requestBody.SetMailNickname(&mailNickname)
description := "String"
requestBody.SetDescription(&description)
createdBy := msgraphsdk.NewIdentitySet()
requestBody.SetCreatedBy(createdBy)
createdBy.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.identitySet",
}
classCode := "String"
requestBody.SetClassCode(&classCode)
externalName := "String"
requestBody.SetExternalName(&externalName)
externalId := "String"
requestBody.SetExternalId(&externalId)
externalSource := "String"
requestBody.SetExternalSource(&externalSource)
externalSourceDetail := "String"
requestBody.SetExternalSourceDetail(&externalSourceDetail)
grade := "String"
requestBody.SetGrade(&grade)
term := msgraphsdk.NewEducationTerm()
requestBody.SetTerm(term)
term.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.educationTerm",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationClass",
}
result, err := graphClient.Education().Classes().Post(requestBody)


```