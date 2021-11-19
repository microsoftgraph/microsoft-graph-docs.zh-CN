---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 50463e023a999e6900a8d0bb825faef2109a9abc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "Holiday event"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.itemAttachment",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
outlookTaskId := "outlookTask-id"
result, err := graphClient.Me().Outlook().TasksById(&outlookTaskId).Attachments().Post(options)


```