---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f64e05e6e64bb3a970014d823670162ef35102b7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327824"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSubjectRightsRequest()
type := "microsoft.graph.subjectRightsRequestType"
requestBody.SetType(&type)
dataSubjectType := "microsoft.graph.dataSubjectType"
requestBody.SetDataSubjectType(&dataSubjectType)
requestBody.SetRegulations( []String {
    "String",
}
displayName := "String"
requestBody.SetDisplayName(&displayName)
description := "String"
requestBody.SetDescription(&description)
internalDueDateTime, err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetInternalDueDateTime(&internalDueDateTime)
dataSubject := msgraphsdk.NewDataSubject()
requestBody.SetDataSubject(dataSubject)
firstName := "String"
dataSubject.SetFirstName(&firstName)
lastName := "String"
dataSubject.SetLastName(&lastName)
email := "String"
dataSubject.SetEmail(&email)
residency := "String"
dataSubject.SetResidency(&residency)
dataSubject.SetAdditionalData(map[string]interface{}{
    "phoneNumber": "String",
    "SSN": "String",
}
result, err := graphClient.Privacy().SubjectRightsRequests().Post(requestBody)


```