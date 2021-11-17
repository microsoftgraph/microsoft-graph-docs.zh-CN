---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3faa4d606b7364e2425b17db729b787dd8aba518
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995798"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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