---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3ce53fab811d688adaeefbc67ece2c51f0e84269
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111518"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
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
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession().Post(options)


```