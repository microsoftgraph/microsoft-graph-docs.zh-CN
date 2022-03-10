---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64ec29fe7361f2a9364cbe258ba0e9f847569376
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411828"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachmentItemRequestBody()
attachmentItem := msgraphsdk.NewAttachmentItem()
requestBody.SetAttachmentItem(attachmentItem)
attachmentType := "file"
attachmentItem.SetAttachmentType(&attachmentType)
name := "scenary"
attachmentItem.SetName(&name)
size := int64(7208534)
attachmentItem.SetSize(&size)
isInline := true
attachmentItem.SetIsInline(&isInline)
contentId := "my_inline_picture"
attachmentItem.SetContentId(&contentId)
options := &msgraphsdk.CreateUploadSessionRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession(message-id).Post(options)


```