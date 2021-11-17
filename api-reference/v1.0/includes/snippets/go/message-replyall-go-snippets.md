---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea7858384adf74ace18d756a9865d8879ce3bbee
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984526"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
options := &msgraphsdk.ReplyAllRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).ReplyAll().Post(options)


```