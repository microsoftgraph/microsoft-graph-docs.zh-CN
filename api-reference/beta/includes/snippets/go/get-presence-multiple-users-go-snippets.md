---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba240ab4a72101bcd534af77413bb217eb7a9af
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100308"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetIds( []String {
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b",
}
options := &msgraphsdk.GetPresencesByUserIdRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Communications().GetPresencesByUserId().Post(options)


```