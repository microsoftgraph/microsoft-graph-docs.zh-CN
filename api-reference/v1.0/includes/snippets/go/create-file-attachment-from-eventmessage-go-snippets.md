---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24cd4693ac7ad1171b4d7a2141596558afa572ff
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328326"
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
    "@odata.type": "microsoft.graph.fileAttachment",
    "contentLocation": "contentLocation-value",
    "contentBytes": "base64-contentBytes-value",
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Post(requestBody)


```