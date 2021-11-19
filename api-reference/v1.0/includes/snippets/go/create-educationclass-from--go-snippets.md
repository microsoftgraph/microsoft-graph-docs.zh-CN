---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f05277ed11d3c800b1f3d665d3ee2a03d137d202
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101352"
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
options := &msgraphsdk.ClassesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Classes().Post(options)


```