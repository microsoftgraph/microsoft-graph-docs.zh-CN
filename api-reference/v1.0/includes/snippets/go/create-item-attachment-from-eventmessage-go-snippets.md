---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29c70a3b0e628badea87cb786c67905963aba8dd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984789"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAttachment()
name := "name-value"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(options)


```