---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ceb264b8ddd150cdf3ffd93ac44dd0f063b2e077
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102857"
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
result, err := graphClient.SharesById(&sharedDriveItemId).Permission().Grant().Post(options)


```