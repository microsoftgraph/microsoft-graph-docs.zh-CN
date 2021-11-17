---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a41adfac077b7b0b05b2003ff5d22151d28845f1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987488"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Members().Post(options)


```