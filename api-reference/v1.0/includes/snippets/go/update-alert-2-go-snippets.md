---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5bd074f75dbe42bce8d997cc40ef4ecc8caea85
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAlert()
assignedTo := "String"
requestBody.SetAssignedTo(&assignedTo)
closedDateTime, err := time.Parse(time.RFC3339, "String (timestamp)")
requestBody.SetClosedDateTime(&closedDateTime)
requestBody.SetComments( []String {
    "String",
}
feedback := "@odata.type: microsoft.graph.alertFeedback"
requestBody.SetFeedback(&feedback)
status := "@odata.type: microsoft.graph.alertStatus"
requestBody.SetStatus(&status)
requestBody.SetTags( []String {
    "String",
}
vendorInformation := msgraphsdk.NewSecurityVendorInformation()
requestBody.SetVendorInformation(vendorInformation)
provider := "String"
vendorInformation.SetProvider(&provider)
vendor := "String"
vendorInformation.SetVendor(&vendor)
headers := map[string]string{
    "Prefer": "return=representation"
}
options := &msgraphsdk.AlertRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
alertId := "alert-id"
graphClient.Security().AlertsById(&alertId).Patch(options)


```