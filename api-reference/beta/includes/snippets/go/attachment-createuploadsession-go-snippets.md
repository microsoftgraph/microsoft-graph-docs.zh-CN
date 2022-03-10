---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7187ebe8f6e351b669cb94e5928284225a16070c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411830"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachmentItemRequestBody()
attachmentItem := msgraphsdk.NewAttachmentItem()
requestBody.SetAttachmentItem(attachmentItem)
attachmentType := "file"
attachmentItem.SetAttachmentType(&attachmentType)
name := "flower"
attachmentItem.SetName(&name)
size := int64(3483322)
attachmentItem.SetSize(&size)
options := &msgraphsdk.CreateUploadSessionRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession(message-id).Post(options)


```