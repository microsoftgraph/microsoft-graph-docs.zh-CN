---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82edde3c5e9af1c0118b87f87d06321f4a3c1c02
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326112"
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
result, err := graphClient.Security().Alerts().UpdateAlerts().Post(requestBody)


```