---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46a0e7ac624b1af9e9a3870988ff47658e6811e1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327335"
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
result, err := graphClient.Education().Schools().Post(requestBody)


```