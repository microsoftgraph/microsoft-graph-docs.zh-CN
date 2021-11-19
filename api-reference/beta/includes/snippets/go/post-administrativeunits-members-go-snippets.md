---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44d08a230054b0cfba9d4f75aefcd48eb0d39aa9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099642"
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
options := &msgraphsdk.MembersRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).Members().Post(options)


```