---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de8fd93ad081910bf043cc7ae3e29dade3181733
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326127"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.Graph.Group",
    "description": "Self help community for golf",
    "displayName": "Golf Assist",
    "groupTypes":  []String {
        "Unified",
    }
    "mailEnabled": true,
    "mailNickname": "golfassist",
    "securityEnabled": false,
}
administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Members().Post(requestBody)


```