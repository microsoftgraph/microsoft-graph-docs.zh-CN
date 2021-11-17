---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bafd806743f2358aef70aedffce65ad92cf61802
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025611"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationSchool()
displayName := "String"
requestBody.SetDisplayName(&displayName)
description := "String"
requestBody.SetDescription(&description)
externalSource := "String"
requestBody.SetExternalSource(&externalSource)
externalSourceDetail := "String"
requestBody.SetExternalSourceDetail(&externalSourceDetail)
principalEmail := "String"
requestBody.SetPrincipalEmail(&principalEmail)
principalName := "String"
requestBody.SetPrincipalName(&principalName)
externalPrincipalId := "String"
requestBody.SetExternalPrincipalId(&externalPrincipalId)
lowestGrade := "String"
requestBody.SetLowestGrade(&lowestGrade)
highestGrade := "String"
requestBody.SetHighestGrade(&highestGrade)
schoolNumber := "String"
requestBody.SetSchoolNumber(&schoolNumber)
externalId := "String"
requestBody.SetExternalId(&externalId)
phone := "String"
requestBody.SetPhone(&phone)
fax := "String"
requestBody.SetFax(&fax)
createdBy := msgraphsdk.NewIdentitySet()
requestBody.SetCreatedBy(createdBy)
createdBy.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.identitySet",
}
address := msgraphsdk.NewPhysicalAddress()
requestBody.SetAddress(address)
address.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.physicalAddress",
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationSchool",
}
options := &msgraphsdk.SchoolsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Education().Schools().Post(options)


```