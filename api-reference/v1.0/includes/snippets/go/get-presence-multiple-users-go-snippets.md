---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74c6565701ebe0a6169d421029dd79d2a9b30d26
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewIdsRequestBody()
requestBody.SetIds( []String {
    "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "66825e03-7ef5-42da-9069-724602c31f6b",
}
options := &msgraphsdk.GetPresencesByUserIdRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Communications().GetPresencesByUserId().Post(options)


```