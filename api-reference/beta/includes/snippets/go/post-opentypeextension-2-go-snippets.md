---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a41e1c603d827600cff29b656838b42a0681c0e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986002"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewExtension()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": ,
    "expirationDate": "2015-12-03T10:00:00.000Z",
}
options := &msgraphsdk.ExtensionsRequestBuilderPostOptions{
    Body: requestBody,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Extensions().Post(options)


```