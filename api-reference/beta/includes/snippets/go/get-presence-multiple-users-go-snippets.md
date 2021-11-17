---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2eb00e1efa416084b2c7f0b37a2420ecc6830dca
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030512"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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