---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae2177776c5a116f90f831b369f786ebca06f14a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60985786"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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
result, err := graphClient.SharesById(&sharedDriveItemId).Permission().Grant().Post(options)


```