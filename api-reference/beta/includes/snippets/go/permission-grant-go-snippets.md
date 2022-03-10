---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ac828623352ea831442aa657bb59b993a5f6b42
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetRecipients( []DriveRecipient {
    msgraphsdk.NewDriveRecipient(),
    SetAdditionalData(map[string]interface{}{
        "email": "john@contoso.com",
    }
    msgraphsdk.NewDriveRecipient(),
    SetAdditionalData(map[string]interface{}{
        "email": "ryan@external.com",
    }
}
requestBody.SetRoles( []String {
    "read",
}
options := &msgraphsdk.GrantRequestBuilderPostOptions{
    Body: requestBody,
}
sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).Permission().Grant(sharedDriveItem-id).Post(options)


```