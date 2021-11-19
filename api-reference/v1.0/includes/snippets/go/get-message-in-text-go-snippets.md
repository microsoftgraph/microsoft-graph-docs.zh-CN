---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3fb36be3463ec4a91f82e2364d72822b1f2d194
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103678"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,uniqueBody",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
    H: headers,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```