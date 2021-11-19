---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6daaf87a9cb51375b736b140ab2dcafb1629a3f7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61095833"
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
options := &msgraphsdk.SubjectRightsRequestsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Privacy().SubjectRightsRequests().Post(options)


```