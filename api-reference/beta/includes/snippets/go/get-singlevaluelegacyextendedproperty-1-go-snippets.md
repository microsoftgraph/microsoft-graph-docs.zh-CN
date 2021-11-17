---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 869ba37c802949d95d47d00a9ffe2ce50f50533f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61002132"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Expand: "singleValueExtendedProperties($filter=id%20eq%20'String%20%7B66f5a359-4659-4830-9070-00047ec6ac6e%7D%20Name%20Color')",
}
options := &msgraphsdk.MessageRequestBuilderGetOptions{
    Q: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Get(options)


```