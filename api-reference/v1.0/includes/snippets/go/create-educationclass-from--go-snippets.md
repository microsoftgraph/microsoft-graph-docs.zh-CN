---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e7cadd3d49f285bf68701922ad005cc6cf50e11
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61031086"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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