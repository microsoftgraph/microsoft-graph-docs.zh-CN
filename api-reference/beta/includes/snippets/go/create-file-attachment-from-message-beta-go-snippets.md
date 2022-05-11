---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66f938e465ceae3f70f4b4a064f6fc646719d634
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328397"
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
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Attachments().Post(requestBody)


```