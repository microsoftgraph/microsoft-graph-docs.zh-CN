---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e673eace25952f082a3ae74f4c51d3fbcab480d1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093797"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "menu.txt"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.fileAttachment",
    "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=",
}
options := &msgraphsdk.AttachmentsRequestBuilderPostOptions{
    Body: requestBody,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(options)


```