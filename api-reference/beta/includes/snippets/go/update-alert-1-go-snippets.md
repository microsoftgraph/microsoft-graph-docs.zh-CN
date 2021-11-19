---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e359617e1bf310beeaf06e8dfea14ed1c31abac2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100447"
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
options := &msgraphsdk.AlertRequestBuilderPatchOptions{
    Body: requestBody,
}
alertId := "alert-id"
graphClient.Security().AlertsById(&alertId).Patch(options)


```