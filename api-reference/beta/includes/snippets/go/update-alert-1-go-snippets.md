---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5342089a6e893af445b91aa5ff21ba5217c0dd9d
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326113"
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
alertId := "alert-id"
graphClient.Security().AlertsById(&alertId).Patch(requestBody)


```