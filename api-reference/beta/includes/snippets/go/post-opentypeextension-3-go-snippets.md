---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f4a18db1bc915665a4dc359f3338b792fcdf505
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986004"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewExtension()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Deal",
    "companyName": "Alpine Skis",
    "dealValue": ,
    "expirationDate": "2015-07-03T13:04:00.000Z",
}
options := &msgraphsdk.ExtensionsRequestBuilderPostOptions{
    Body: requestBody,
}
groupId := "group-id"
eventId := "event-id"
result, err := graphClient.GroupsById(&groupId).EventsById(&eventId).Extensions().Post(options)


```