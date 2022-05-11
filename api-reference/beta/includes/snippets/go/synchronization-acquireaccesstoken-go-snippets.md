---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3303096c72dd45c4b129d2d22774bd8ee8d32b5a
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCredentialsRequestBody()
requestBody.SetCredentials( []SynchronizationSecretKeyStringValuePair {
    msgraphsdk.NewSynchronizationSecretKeyStringValuePair(),
    SetAdditionalData(map[string]interface{}{
        "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair",
    }
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Synchronization().AcquireAccessToken(application-id).Post(requestBody)


```