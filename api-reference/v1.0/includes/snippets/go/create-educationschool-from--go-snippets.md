---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80d8692cbb4fdbb78602e8ad17b3b123182e5bae
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61094691"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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