---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acfd1ad708fcf508c3f8d14c521f11dbc3347ab2
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61096519"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "menu.txt"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "contentBytes": "base64bWFjIGFuZCBjaGVlc2UgdG9kYXk=",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(options)


```