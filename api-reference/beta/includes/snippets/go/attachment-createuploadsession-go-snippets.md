---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 45380bb006151c183bfabbfa8a68549d552f5ece
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60982552"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
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
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession().Post(options)


```