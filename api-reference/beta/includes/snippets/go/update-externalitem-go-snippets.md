---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bf9f518b526e07491f180cfb5c1ee82b1980cbf
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396033"
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
options := &msgraphsdk.ExternalItemRequestBuilderPatchOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Patch(options)


```