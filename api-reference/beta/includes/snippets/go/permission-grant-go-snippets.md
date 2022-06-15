---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75e2675c22b3b1de3945a9a9bbdf2b2d5cdaaee6
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098673"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetRecipients( []DriveRecipient {
    msgraphsdk.NewDriveRecipient(),
email := "john@contoso.com"
    SetEmail(&email)
    msgraphsdk.NewDriveRecipient(),
email := "ryan@external.com"
    SetEmail(&email)
}
requestBody.SetRoles( []String {
    "read",
}
sharedDriveItemId := "sharedDriveItem-id"
result, err := graphClient.SharesById(&sharedDriveItemId).Permission().Grant(sharedDriveItem-id).Post(requestBody)


```