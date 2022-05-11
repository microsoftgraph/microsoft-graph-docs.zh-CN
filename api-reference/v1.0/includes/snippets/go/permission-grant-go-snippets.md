---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7492f7ec5ebebba6aa56f08788eed6a8e99097b5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328030"
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
sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).Permission().Grant(sharedDriveItem-id).Post(requestBody)


```