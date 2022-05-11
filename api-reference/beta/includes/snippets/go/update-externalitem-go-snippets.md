---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c13cd8fac916f518f5236a2443f8551c8ab4e5b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326266"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalItem()
requestBody.SetAcl( []Acl {
    msgraphsdk.NewAcl(),
    SetAdditionalData(map[string]interface{}{
        "type": "everyone",
        "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
        "accessType": "grant",
    }
}
externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Patch(requestBody)


```