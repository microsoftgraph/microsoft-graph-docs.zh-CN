---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 818c7d5da1ba92ea29d967fd1a84158d5a952703
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326832"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExtension()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.openTypeExtension",
    "extensionName": "Com.Contoso.Referral",
    "companyName": "Wingtip Toys",
    "dealValue": ,
    "expirationDate": "2015-12-03T10:00:00.000Z",
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).Extensions().Post(requestBody)


```