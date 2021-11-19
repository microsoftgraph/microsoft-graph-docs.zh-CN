---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4e6309f4fa04dd0c2c7164f35e0ed30157365bd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
comment := "comment-value"
requestBody.SetComment(&comment)
options := &msgraphsdk.ReplyAllRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
graphClient.Me().MessagesById(&messageId).ReplyAll().Post(options)


```