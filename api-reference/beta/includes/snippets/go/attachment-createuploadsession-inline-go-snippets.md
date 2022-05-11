---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e17560a5fa0fc103ff9e7c946ce7c1b4bdf0664
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326943"
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
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().CreateUploadSession(message-id).Post(requestBody)


```