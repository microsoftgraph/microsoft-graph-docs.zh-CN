---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8236da0b33cbdbd342cd3e76524533dfcabcc5cf
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60993535"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
deviceId := "device-id"
result, err := graphClient.DevicesById(&deviceId).RegisteredOwners().$ref().Post(options)


```