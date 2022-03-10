---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93b3939d7eea2020d60a9eeaceb2b5805bcd924e
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412086"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewValueRequestBody()
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