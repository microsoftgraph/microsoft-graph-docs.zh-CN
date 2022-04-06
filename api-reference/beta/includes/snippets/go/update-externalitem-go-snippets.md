---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e452a88c4c9b460c5fd81a006db84f89924c30e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528076"
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
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Patch(options)


```