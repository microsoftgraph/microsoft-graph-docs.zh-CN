---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 783ee5be49811aaaececcd7a6faf2238c75de4fe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328857"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "name-value"
requestBody.SetName(&name)
contentType := "contentType-value"
requestBody.SetContentType(&contentType)
isInline := false
requestBody.SetIsInline(&isInline)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.OutlookServices.FileAttachment",
    "contentLocation": "contentLocation-value",
    "contentBytes": "contentBytes-value",
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Post(requestBody)


```