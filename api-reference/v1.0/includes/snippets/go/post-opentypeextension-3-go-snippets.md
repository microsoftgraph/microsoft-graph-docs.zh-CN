---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a39e4970f4ba6a7e4326154bfb778e205c35a939
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61081982"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

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