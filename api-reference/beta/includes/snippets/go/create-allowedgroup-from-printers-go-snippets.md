---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eaf3cf81b7f21de78a85c38f01c888b492db0677
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61100574"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/groups/{id}",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).AllowedGroups().$ref().Post(options)


```