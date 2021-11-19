---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3dbffb99d5b428fa4b274f839fc3b7f70947083a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102704"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
message := msgraphsdk.NewMessage()
requestBody.SetMessage(message)
message.SetAdditionalData(map[string]interface{}{
    "isDeliveryReceiptRequested": true,
    "toRecipients":  []Object {
    }
}
comment := "Dana, just want to make sure you get this; you'll need this if the project gets approved."
requestBody.SetComment(&comment)
options := &msgraphsdk.CreateForwardRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateForward().Post(options)


```