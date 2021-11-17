---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1107c111871e5b9dc4d4450dd31db919b7fcbae0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61010582"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetCredentials( []SynchronizationSecretKeyStringValuePair {
    msgraphsdk.NewSynchronizationSecretKeyStringValuePair(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
    }
}
options := &msgraphsdk.AcquireAccessTokenRequestBuilderPostOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Synchronization().AcquireAccessToken().Post(options)


```