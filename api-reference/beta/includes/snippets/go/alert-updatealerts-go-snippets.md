---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00931dabdd3e12f1630086f4e74e808f3a8c18b3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991107"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetValue( []Alert {
    msgraphsdk.NewAlert(),
    SetAdditionalData(map[string]interface{}{
        "assignedTo": "String",
        "closedDateTime": "String (timestamp)",
        "comments":  []String {
            "String",
        }
        "id": "String (identifier)",
        "tags":  []String {
            "String",
        }
    }
}
options := &msgraphsdk.UpdateAlertsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Security().Alerts().UpdateAlerts().Post(options)


```