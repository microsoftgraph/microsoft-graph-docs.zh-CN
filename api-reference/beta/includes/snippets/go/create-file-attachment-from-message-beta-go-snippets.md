---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 347ded9d3362fb2c4696a72a7bb1d1c98850e749
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083794"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "smile"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "contentBytes": "a0b1c76de9f7=",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Post(options)


```