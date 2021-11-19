---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9be7c172ad21b943df7ac63f2bcaa771bb6ff0f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103437"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAdditionalData(map[string]interface{}{
    "attachments":  []Object {
    }
}
comment := "if the project gets approved, please take a look at the attached guidelines before you decide on the name."
requestBody.SetComment(&comment)
options := &msgraphsdk.CreateReplyAllRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateReplyAll().Post(options)


```